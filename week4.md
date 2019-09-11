# Week 4


#### MC1

Q: BabelJS does which of the following...

* Compiling
* Interpreting
* Transpiling
* Mansplaining

#### MC2

Q: A function which wraps a callback and counts the number of times it is invoked is called what?

* A Mock
* A Spy
* A Monad
* A Stub


#### MC3

Q: Which method is not accessible from the Redux Store?

* subscribe()
* getState()
* unsubscribe()
* dispatch()

#### MC4

Q: Which is not a good use-case for Redux?

* A browser-based game with lots of async user events
* An ecommerce store that tracks user authentication across views
* A dashboard that updates a series of graphs in real time
* A fan wiki where users can read hundreds of articles

A: The fan wiki. Redux excels in projects that have many dynamic state changes over time, because it allows to manage those changes in a declarative, predictable way. This is why Redux is a good choice for games, or for complex dashboards. Redux (along with React-Redux) also provides an easy way to share state amongst many components, regardless of where they are in the view tree - this is why Redux would also be helpful for an ecommerce store that tracks user authentication. Otherwise, the logged in user would need to be passed down as prop throughout the entire render tree, which could be tedious. The fan wiki, however, is not very dynamic - it simply has pages that users read, without a whole lot of interaction. Redux would be overkill for an app like that, and possibly hinder more than help.

#### SA1

Q: What are the three main components that we import from react-router-dom, and what do they do?

A: Router, Route and Link. The Router contains all of the state about the url bar, and causes all of its children to re-render when the url changes. A Route will conditionally render a component if the url matches the given path. Links are used to make navigable links that users can click on.

#### SA2

Q: Describe the difference between a “controlled” input, and an “uncontrolled” input. What is the advantage/disadvantage of each?

A: A “controlled” input has its “value” prop set to a value from state. To update the value in the form, the value on state must also be updated (usually via an onChange handler). This allows us to change the value in the form programmatically by setting state. The downside is that we have to write more code. An “uncontrolled” input does not have its value controlled by state - we simply extract the values from the DOM when we submit. This means we can write a lot less code. However, the downside is that we can’t programmatically control what displays in the form.

#### SA3

Q: Describe the three rules of Redux

A: Redux has a single reference to the application’s state it keeps in the store. The view state is immutable, and whenever the store must update the state, a new state object is created. The functions which dispatch actions to the store in order to create an update state are also pure, meaning they have no side-effects.