SEQUELIZE is a promise-based Object/Relational Mapper and JavaScript library that can be used to communicate with databases. To use it, it is necessary to install it with the NPM and require it in the main JS file like so:
```js
var Sequelize = require('sequelize')
```
To access the database, the following code is used:
```js
var sequelize = new Sequelize('database', 'username', 'password')
```
To create a table, one must first define the property names and data types of the values to be created:
```js
var User = sequelize.define('user', {
  username: Sequelize.STRING,
  birthday: Sequelize.DATE
});
```
After that, it can be updated with the following syntax:
```js
sequelize.sync().then(function() {
  return User.create({
    username: 'janedoe',
    birthday: new Date(1980, 6, 20)
  });
}).then(function(jane) {
  console.log(jane.get({
    plain: true
  }));
});
```

