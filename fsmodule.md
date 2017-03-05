THE FILE SYSTEM MODULE is a native JavaScript module, so you don't have to use Node Package Manager to install it to your app. To use it, all you need to do is require it like so:
```js
fs = require('fs')
```

To read a file, follow this syntax:
```js 
fs.readFile('/filename', 'utf8'/*or other encoding*/, (err, data) => {
    if (err) throw err
    console.log('Contents of file: ' + data)
    })
```

To write a file, follow this syntax:
```js
fs.writeFile('/filename', 'new content', (err) => {
  if (err) throw err;
  console.log('File written!');
});