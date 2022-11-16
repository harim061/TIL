# 2. React Intro
## 2-1. React Intro
- React is a JS library for building User interfaces
- only responsible for the view layer of your application 
    - it is only responsible for rendering your User Interface as well as updating the UI whenever it changes
- allows to reuse this logic in another part of your UI

### is NOT a framework
-  library only helps you in one aspect. In contrast, a framework helps you in many aspects

### 💡Recap
1. React is a JS library for building UI
2. React is only responsible for the View layer
3. React is not a framework

## 2-2. install & setup
```
npm install react
```

### importing React
```
import React from "react";
```
- React is not part of the browser, so you must import it
- default import following syntax : import Something from "package-name"

### The React object
- you get a React object that contains methods and properties

💡Recap : object
> unordered collection of data in the form of key : value pairs.
```
const person = {
   first_name: "Sam",
   last_name: "Doe",
   age: 29
};
```

## 2-3. Document.createElement
> document.createElement(tagName) is a Web API provided by browsers that let you programmatically create an HTML element

- it creates an HTML element.
- console.dir(element) : can see all the properties by using this
- id, style, className

### Multiple classes
> can be set by separtaing the class names with a space character

```
const element = document.createElement("h2"); // h2태그 생성
element.className = "container center";
// <h2 class ="container center"></h2>
```
## 2-4. React.createElement
- React.createElement and document.createElement is not the same thing
> React.createElement returns an object that represents the DOM element

```
const element = React.createElement("h1");
//returns an object similar to this one:
{
  type: 'h1',
  props: {}
}

```
- because React operates a Virtual DOM
```
React.createElement("h1",{classNmae:"center",style:"color:red"})
```
### Writing text
- to write you have to provide the 3rd parameter 
```
React.createElement("h1", {}, "Hello World")
```
- we don't want to set a className or style -> {} as the second parameter

### What is a React Element?
> the smallest building block

