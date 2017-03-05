EXPRESS is a minimal and flexible web application framework for Node.js that simplifies development and makes it easier to write secure, modular, and fast applications. You must install it with NPM and then require it to your app like so in order to use it:
```js
const express = require('express')
```
Additionally, it is required to add this line of code to create your app from the library:
```js
const app = express()
```
An example of a simple route used in express:
```js
app.get('/', function(res, res) {
    res.send("Hello World!")
    })
```
To serve static files like images, CSS, and JS files, you can use the express.static built-in middleware function. Pass the name of the directory that contains the static assets to start serving the files directly:
```js
app.us(express.static('public'))