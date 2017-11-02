# HTML-Templating-Engine

Completely replaces the need to use HTML.

# Installation

Place htmlEngine.js inside of your main HTML document.

````html
<html>
  <head>
    <meta charset="utf-8">
  </head>
  <body>
    <script src="htmlEngine.js"></script>
  </body>
</html
````

# Usage

Append elements to the DOM using JS

Parameter one is the elements tag (ie. div, img, li)

Parameter two is the elements class name.

Parameter three is the existing element to append to.

````javascript
create('div','className','appendToElement');
````
The fourth parameter is optional. An 'a' will append  your new element to all elements with the name given for parameter three. A numeric value will append your element to the element given for parameter three with that index; if the element doesn't exist a number of elements equal to that number will be created and appended to the third parameter.

```javascript
//append the element className to all elements named appendToElement

create('div','className','appendToElement','a');

//append the element className to the 2nd occuring element named appendToElement

create('div','className','appendToElement',1);
````
