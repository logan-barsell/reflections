JQUERY is a JavaScript library that simplifies JS programming. To use it, you must download the jQuery files and link it in your HTML file:
```html
<script src="./jquery.js"></script>
```
The syntax for jQuery goes as follows:
```js
//EXAMPLE
$(document).ready(function(){
    //When the p tag is clicked, jQuery will hide the element
    $("p").click(function(){
        $(this).hide();
    });
});
```

