A PROMISE represents the eventual result of an asynchronous operation and acts as a placeholder into which the successful result value or reason for failure will materialize. It is a function passed with the arguments resolve and reject which are functions that are called depending on whether or not the promise was resolved or rejected. The syntax is as follows:
```js
var promisefunct = new Promise(function(resolve, reject) {
    if(/*good condition*/){
        resolve('Success!')
    }
    else {
        reject('Failure!')
    }
    })
```
It can then be chained with then() and catch() methods
```js
promisefunct.then(function(){
    /*do something here*/
}).catch(function(){
    /*error*/
})