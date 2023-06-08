# React

**Script to creat a new proyect in React in the Terminal of VS Code after creating a folder:

NPX create-react-app
name-of-the-new-folder  **Enter

Later, I am able to create components depending on my proyect:

**Example:

components.JS
or
componets.JSX in case I want to use JS and React mixed.

import React from "react";

> Lets start with the first functional container:

funtion Testiomonial() {
return (
<div className='conetendor-testimonio'>
 <img
      className='imagen-testimonio'
      src={require('../imagenes/testimonio-emma.png')}
      alt='Foto de Emma' />
</div>)
}
**This is to make blank our website=
**To start adding this content to our new Website, we need to remove "setupTest.js, reportWebVitals.js, App.test.js" from React.

**From index.js we should delete "import reportWebVitals from './reportWebVitals' and reportWebVitals();

**At App.js we will keep the <div ClassName="App"> </div> **And delete everything inside this Div.

**At App.css we will delete everything inside not the file. 




** Script to creat a component and render it**

class MyComponent extends React.Component{
  constructor(props) {
    super(props);
  }
  render() {
    return (
      <div>
      <h1>My First React Component!</h1>
      </div>
    )
  }
}

ReactDOM.render(<MyComponent />, document.getElementById('challenge-node'))
