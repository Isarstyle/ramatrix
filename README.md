[![Stories in Ready](https://badge.waffle.io/jhyman2/ramatrix.png?label=ready&title=Ready)](https://waffle.io/jhyman2/ramatrix)
# Ramatrix (React Availability Matrix)

> A react component to gather a user's hourly availability.

## Install
```
npm install ramatrix --save
```

## Usage within a React component
```
import Ramatrix from 'ramatrix';

// call this function when you want to get the matrix data
getMatrixData () {
  console.log(this._myMatrix.getData()); // "{"7AMTh":true,"8AMTh":true.....
}

render () {
  return (
    <Ramatrix ref={(c) => this._myMatrix = c}/>
  );
}
```

## Customizable options
Props can be passed for data and styling customization

`militaryTime - boolean (true/false) | default - false`
 - Will display hours from 0 - 23 or 12AM - 12PM

`containerStyle - reactStyling object | default - display: inline-block;`
 - styling that will be applied to outer container

`cellWidth - reactStyling object | default - 65px`
 - width that will be applied to individual cells

`customID - string | default - 'RAM-container'`
 - id assigned to parent div of component

`tableClassName - string | default - 'RAM-table'`
 - className of the table element

`tableHeadName - string | default - 'RAM-header'`
 - className of the table head element

`tableBodyName - string | default - 'RAM-body'`
 - className of the table body element

![SSS1](https://github.com/jhyman2/ramatrix/blob/master/screenshot.png?raw=true)

## Contribute/Development
<h3>Compiling for development</h3>

Simply run `npm install` and `npm run dev` from the root of the project.  This will run webpack-dev-server on port 8080.

<h3>Preview in a browser!</h3>
```
localhost:8080
```

<h2>Authors</h2>
* [jhyman2](https://github.com/jhyman2)
* [kevcoxe](https://github.com/kevcoxe)

<h2>Links</h2>
* [git repo](https://github.com/jhyman2/ramatrix)
* [npm](https://www.npmjs.com/package/ramatrix)