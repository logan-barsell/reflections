ANONYMOUS CALLBACK FUNCTIONS are unnamed functions that are passed into other functions as a parameter. The general idea behind it is "after this, do that".
The syntax goes as follows:
```js 
var friends = ["Mike", "Stacy", "Andy", "Rick"];
​
friends.forEach(function (eachName, index){
console.log(index + 1 + ". " + eachName); // 1. Mike, 2. Stacy, 3. Andy, 4. Rick​
});
```

