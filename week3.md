# Week 3

#### MC1

Q: Which of the following describes a test that tests only a single, isolated piece of code?

* Integration test
* Unit test
* Function test
* User test

#### MC2

Q: Which of the following is a strategy for managing async code in the mocha/chai test framework? Select ALL THAT APPLY.

* Invoke the “done” callback once all of the expect blocks are completed
* Return the value done once all of the expect blocks are completed
* Return a promise from the it block that will resolve only once all the expect statements have completed
* Use async/await with your it blocks

#### MC3

Q: Which of the following is NOT a valid React component?


 
```javascript
const Foo = () => {
  return <div></div>
}
```


```javascript
class Foo {
  render () {
    return <div></div>
  }
}
```


```javascript
export default (props) => {
  return <div></div>
}
```


```javascript
class Foo extends React.Component {
  render () {
    return <div></div>
  }
```

#### MC4

Q: Which the following are appropriate ways to access props in a component? Select ALL THAT APPLY.

* In a stateless functional component, get the props object from the first argument to the function
* In a stateless functional component, get the props object from this context (i.e. this.props)
* In a class component, get the props object from this context (i.e. this.props)
* In a class component, get the props object from the first argument to the render method


#### SA1

Q: In your own words, describe the TDD process.

A: First, consider possible input/output for your function. Then, write a small, failing test for that function. Write the minimal amount of code necessary to make that test pass. Temporarily break your code to make sure that the test fails (this ensures that you aren’t getting a false positive). Fix your code and ensure you pass the test again. Then repeat the process.

#### SA2

Q: In your own words, describe the componentDidMount() React Lifecycle Method

A: After a Component received props, is rendered, and mounted to the DOM, the componentDidMount() lifecycle hook will fire. This is an ideal place for any async functions such as making an AJAX request or subscribing to the Redux store, because it will not interfere with the component’s rendering in the client’s browser.