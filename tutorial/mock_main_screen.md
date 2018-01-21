# Bird Snap

## Mocking the Main Screen
A simple way to get started is to use plain HTML and CSS to mock the screen.

The only component in the application is *App* found in the file __src/App.js__.
If you open that file in your favourite editor you will see the following code:

```jsx harmony
import React, { Component } from 'react';
import logo from './logo.svg';
import './App.css';

class App extends Component {
  render() {
    return (
      <div className="App">
        <header className="App-header">
          <img src={logo} className="App-logo" alt="logo" />
          <h1 className="App-title">Welcome to React</h1>
        </header>
        <p className="App-intro">
          To get started, edit <code>src/App.js</code> and save to reload.
        </p>
      </div>
    );
  }
}

export default App;
```

### What you see
1. The first three lines are import statements used to make other components and
JavaScript modules available for use in this file.
  - React and { Component } are imported from the *react* package. React is necessary
  for the JSX code written later in the file to compile properly. Component is
  the base class for all React components.
  - logo is an svg image used to make teh spinning logo that you see on the app
  - __App.css__ is the CSS code applied to this component.
2. The next line of code starts a class representing the component that you are building.
Most of the code that you write for a component will be in the class block.
3. The *render()* method is the only required method in a React component. It returns the JSX that defines the UI. Notice that 
the code between the parentheses of the `return` statement look like plain old HTML. That is [JSX](https://reactjs.org/docs/introducing-jsx.html) which for the most part behaves just like HTML but is much more. 
We will be highlighting the differences as we encounter them later.
    

### Make Your Own Screen
Edit the JSX code and add your own layout as you would like. For example

```jsx harmony
    return (
      <div className="App">
        <h1>Welcome to Bird Snap</h1>
        <p>We are going to have fun!</p>
      </div>
    );
```
