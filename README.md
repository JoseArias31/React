# React

**Script to creat a new proyect in React in the Terminal of VS Code after creating a folder:

NPX create-react-app
name-of-the-new-folder  **Enter

Later, I am able to create components depending on my proyect:

**Example:

components.JS
or
componets.JSX in case I want to use JS and React mixed.

**import React from "react";

> Lets start with the first functional container:

funtion Testimonio() {
return (
<div className='conetendor-testimonio'>
 <img
      className='imagen-testimonio'
      src={require('../imagenes/testimonio-emma.png')}
      alt='Foto de Emma' />
 <div className='contenedor-texto-testimonio'>
  <p> className='nombre-testimonio'>Jose Arias from Colombia</p>
  <p> className='cargo-testimonio'>Full Stack Web Develover</p>
  <p> className='texto-testimonio'>Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.</p>
  </div>
</div>)
}
**This is to make blank our website=
**To start adding this content to our new Website, we need to remove "setupTest.js, reportWebVitals.js, App.test.js" from React.

**From index.js we should delete "import reportWebVitals from './reportWebVitals' and reportWebVitals();

**At App.js we will keep the <div ClassName="App"> </div> **And delete everything inside this Div.

**At App.css we will delete everything inside not the file. 

**ONCE the component is ready, we need to import it from "App.js" like this:
<div ClassName="App">
<Testimonio />
</div>

**And on the top where the import section is, we need to import the .JS file like this:

**import Testimonio(name of the component) from './componentes/Testimonio.js(where the file is located)'

**To make this file appears on the website, we need to export it from the Component file at the end of the code:

**export default Testimonio;


**PROPS
Here, we use props to replace contect instead of copu a paste every component. 
**
funtion Testimonio(**props) {
return (
<div className='conetendor-testimonio'>
 <img
      className='imagen-testimonio'
      src={require('../imagenes/testimonio-emma.png')}
      alt='Foto de Emma' />
 <div className='contenedor-texto-testimonio'>
  <p> className='nombre-testimonio'>Jose Arias from Colombia</p>
  <p> className='cargo-testimonio'>Full Stack Web Develover</p>
  <p> className='texto-testimonio'>Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.</p>
  </div>
</div>)
}












**Example:Script to creat a component and render it**

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
