COOKIES are data, stored in small text files, on your computer. When a browser requests a web page from a server, cookies belonging to the page is added to the request. This way the server gets the necessary data to "remember" information about users.
The first thing you should do is use NPM to install cookie-parser to your app, then require it in the main JS file like so:
```js
const cookieParser = require('cookie-parser')
```
It is also necessary to add the following code:
```js
app.use(cookieParser())
```
Next, to make your life much easier, download js.cookie.js from https://github.com/js-cookie/js-cookie, place it in your static files, and link it to your HTML file as follows:
```html
<script src="js.cookie.js"></script>
```
Finally, to make your cookies, follow this syntax:
```js
if (Cookies.get('visited')) {
//In this case, text is inserted into the HTML file
document.getElementById('hasvisited').innerHTML = "Hello, cookie have been activated!"
}
Cookies.set('visited', true)
```
