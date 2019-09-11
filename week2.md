# Week 2


## Quiz Questions

#### MC1

Q: What does the following code log to the console (do not run this code in a repl - reason about it on your own):

```javascript
console.log(‘hello’)
setTimeout(() => {
  console.log(‘world’)
}, 0)
console.log(‘goodbye’)
```

* hello, world, goodbye
* hello, goodbye, world
* goodbye, world, hello
* world, hello, goodbye

#### MC2

Q: Which of the following is NOT a BUILT-IN Node module?

* http
* fs
* express
* path

##### MC3

Q: What is the advantage of performing a “Big O” analysis on an algorithm?

* To benchmark the actual time it takes for an algorithm to run
* To determine if one algorithm is better than another
* To decide between heuristics when trying to come up with practical solutions to normally intractable problems
* To compare the growth curves of algorithms as their input sizes get very, very large

#### MC4

Q: What is the purpose of the package.json file in a Node project?

* Store a list of dependencies for the project
* Give the project a name
* Store metadata about the project
* All of the above
* None of the above

#### MC5

Q: Which of the following Express route handlers will be executed for a request like GET /puppies HTTP/1.1. Select ALL THAT APPLY.

```
A: app.use((req, res) => {})
B: app.get(‘/’, (req, res) => {})
C: app.get(‘/puppies’, (req, res) => {})
D: app.use(‘/’, (req, res) => {})
```

##### MC6

Q: Assume we have two SQL tables: Dinos and Bones. Which of the following will add a dino_id to the Bones table?

* Bone.belongsTo(Dino)
* Dino.hasMany(Bone)
* Bone.hasMany(Dino)
* Dino.belongsTo(Bone)

#### SA1

Q: In as much detail as possible, describe what happens when you require a module in Node (ex. require(‘./someFile’))

A: If the module being required has not been required before, it is executed and the module.exports of that module is calculated, and cached. The value of module.exports is then returned from the call to require. If the module being required HAS been required before, the cached value of module.exports is returned without executing the module again.

