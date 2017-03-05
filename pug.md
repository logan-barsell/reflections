PUG is a view/template engine, which replaces variables in a template file with actual values and transforms the template into an HTML file sent to the client. You must use NPM to install it to your app, then require it like so:
```js
const pug = require('pug')
```
To use pug, you must also set the view engine to pug in your main JS file:
```js
app.set('view engine', 'pug')
```
After the view engine is set, create a pug template file named index.pug in a directory called views. The syntax goes as follows:
```pug
html
    head
        title= title
    body
        h1= message    
```
To render the file, you need to create a route in your main JS file:
```js
app.get('/', function (req, res) {
  res.render('index')
})
```
