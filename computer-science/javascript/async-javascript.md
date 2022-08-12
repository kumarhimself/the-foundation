# Asynchronous JavaScript
#computer-science #programming #javascript

## Introduction
 - Best described as the ability to run other tasks while running a program
 - By default, JavaScript can only run one statement at a time from top to bottom
	 - Called a single-threaded language
	 - Can become a problem if each statement takes some time to complete
		 - That's where asynchronous JavaScript comes in
 - Solution to synchronous systems is to start additional threads of control
	 - Thread - another running program whose execution may be interleaved with other programs

### Callback Functions
 - Functions that are used as arguments in another function and are only executed after the main action is done
 - An example of this is the SetTimeout function:
	```javascript
	setTimeout(() => {
		console.log("Waited 2 seconds");
	}, 2000);
	```
 - A unamed arrow function is taken as a argument in the `SetTimeout` function

### Promises
 - An asynchronous action that may be completed at some point and produce a value
 - Easiest way to create a promise is by calling `Promise.resolve` 
	 - Ensures that the value you give is wrapped in a promise
	 - If it is already a promise, it is simply returned, otherwise, you get a new promise that immediately finishes with your value as its result
 - To get the result of a promise, you can use the `then` method, which registers a callback function to be called when the promise resolves and produces a value
	 - Can add multiple callbacks to a single promise, and they will be called, even if you add them after the promise has already been resolved (finished)
 - Example:
```javascript
let fifteen = Promise.resolve(15);
fifteen.then(value => {
	console.log(`Got ${value}!`)
});
```

