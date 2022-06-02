React :

features of React React v/s angular v/s vue Why you chose react why react is so powerful

JS library developed by Facebook SPA - single page application : Any web application , in which when you are clicking on any button or selecting option from navigation bar then if your page which means browser page is reloading then that means that application is your multi - page application . If it does not reload the browser page and just only updates the page without reloading then that application is known as Single Page application. When you create React application using CRA, (create-react-app boilerplate , developed by Facebook) it always create the application which will be Single page application.

component structure : Whenever we are creating React application so the complete screen component will be broke down into smaller components. We do this thing to make sure that these components can be reused at any time when required. React we have two different types of components : Class and Functional. In React we also create smart and dumb components. Smart are the ones in which state variable is there and you can do all the data manipulation in this. Dumb are the ones which only used for UI, they receive data from parent component as props.

Virtual DOM : DOM is a document object model, created by converting HTML CSS and JS Real DOM, which is an object which gets created whenever any React application gets loaded on the screen for the first time., whenever React components gets mounted on the screen for the first time. Now when any user makes any changes on the screen like button click because of which the state variable will get updated so in this case the changes will not directly go to Real DOM , instead in react we have concept known Virtual DOM. So we are having two virtual doms, one virtual dom gets created at the time of mounting of react component so it is a copy of your real dom. Another virtual dom is the dom which contains the new changes, updated state variables values. Now these two virtual doms will get compared with each other and will check for the new changes. this complete procedure is known as diffing algorithm. Now the new changes will be updated in your Real dom. this procedure is known as Recoinciliation.

Good community support :

Build User interface : used to build Front-end application JSX : Initially when React developed it was pure JS library in which we were able to write only JS inside a component. To add HTML on webpage React used React.createElement function. But this function was getting complex when you want to build big web pages. Later React introduced JSX which allowed us to write HTML and JS in a single file.

Easy learning curve : It requires only the knowledge of Javascript. But in case of Angular it requires Typescript.

React Native : Using React we can create mobile - application as well which supports both Android and iOS.

Client Side rendering one way binding

Library v/s Framework :Library is a collection of functions :Framework is a collection of multiple other libraries. :Inversion of Control = In case of library the Execution of code will be decided by the developers whereas in case of framework the execution is already defined or decided. :In case of Framework, it follows MVC structure (model view controller) whereas a library can only be the one for example React is View of MVC :Framework provides you a structure in which you just put down the code your functionality , in case of library its developers duty to design the structure.

Readme.md : MarkDown Documentation= md This contains information about the project that which file contains what information and also contains info like how a new person who is starting with the project how they have to start with the project

package.json : It contains the information about the project and also contains the libraries which the project is using and it also has the description of the commands which gets used to run test or build your project.

package-lock.json : It contains information about the major libraries and if these libraries are having any extra dependency on other libraries so that information will also be stored over here.

.gitignore: we can list down all the folders or file which we do not want to push during pushing the changes in github like node_modules.

public/index.html: this file contains one div element in which a id is stored which is used to render your complete application at this id

src/index.js : In this file you will render your complete React application at the id given in index.html file.

src/App.js : From this file ,developers can start building their React application

Babel: It is a transcompiler. Firstly, It converts the JSX into JS and then it converts ES6 code to ES5 so that browser can understand.

Webpack: It is a type of bundler. It takes all the HTML, CSS and JS code and reducves the size of bundle so that it can be loaded on the browser.

Q: How many imports are there in React JS?
Ans- default and named. How will import a component depends on how you have exported that.

Q: How to create a state variable in class component?
import React from "react"
class App extends React.Component{
state = {
name: "Abhijeet"
}
render(){
return(
<div>Hello{this.state.name}</div>
)
}
}
export default App

We can also write like this,
import React, {Component} from "react";
class App extends Component{
}



In React we have two types of components : class and funtional

We are moving from class components to functional components in React because :

    Class components have a proper structure like constructor and this keyword which is tricky to use , in case of fucntional component we dont have to follow any such structure.
    Since JS is a functional programming language , so classes are not that much preferred
    Functional component is faster in execution compared to class

This application contains the introduction and code to understand the Hooks got introduced in React 16.8 version .

   1. useState = User.js
   2. useEffect = User.js
   3. useContext = Students.js and context.js
   4. useReducer = CompReducer.js
   5. useRef = CompReducer.js
   6. useMemo = Memo&Callback folder
   7. useCallback = Memo&Callback folder

Other than hooks, it contains the introduction of how to setup context API in React project

This also contains a little explanation about Login authentication and authorization , means how to pass the JWT token in the API and also contains one socket folder explaining how to make socket connection from front-end .

