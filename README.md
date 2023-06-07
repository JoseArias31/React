# React

** Script to creat a new proyect in React in the Terminal of VS Code after creating a folder:

NPX create-react-app
name-of-the-new-folder  **Enter

Later, I am able to create components depending on my proyect:

Example:

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
      alt='Foto de Emma'
</div>)
}

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
