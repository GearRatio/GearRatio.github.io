#  HTML and CSS, Tables & Functions Method and Objects from JS Book

## Tables
Tables are created using the `<table>`, `<tr>` (table row), `<td>` (table data), and `<th>` (table header) elements. It is important to use the `<th>` element so screen readers are able to understand the information that is stored within. You can span rows and columns using `colspan` or `rowspan` attributes. These are placed opening tag of the specified element to span.

There are  also three main elements that should be considered using with accessibility  in mind. They are `<thead>`, `<tbody>`, `<tfoot>`. These elements are also used to splint a long table into sections.

Basic Structure
```html
<table>
  <tr>
    <th>vertical 1</th>
    <th>vertical 2</th>
    <th>Table head 3</th>
  </tr>
  <tr>
    <th>horizontal 1</th>
    <th>horizontal 1</th>
    <th>horizontal 1</th>
  </tr>
  </table>
```

## Functions Method and Objects
You can create an object in two ways, either by literal notation or by using constructor notation. By using the term `new` JavaScript creates an instance of an object that has a constructor function. Objects are made up of `key` and `value` pairs. All keys in an object must be unique.

Literal Example:
```js
var shoe = {
  brand: 'Nike',
  color: 'white',
  size: 12,
  quantity: 6,
}
```

Constructor Example:
```js
var shoe = new Object();
shoe.brand ='Nike';
shoe.color = 'white';
shoe.size = 12;
shoe.quantity = 6;
```
Once an object has been created, either with literal or constructor, you can add new properties it using dot notation. You can also `delete` properties by simply delete shoe.color.

The keyword `this` is commonly used inside functions and objects. When a function is declared `this` is altered and only refers to one object, usually within the function scope itself. 

Functions created at the top of the script that are not inside other objects or functions are considered `Global` functions. The same principal can be applied to variables.

When a function is defined within an object, it becomes a method. In a method *this* refers to the containing object.

Objects are perfect for storing data. Objects can hold other objects, arrays, and functions. Arrays are a type of an object and can be accessed with in an object using bracket notation.

Additionally, JavaScript has three main groups of built in Objects.
* Browser Object Model
* Document Object Model
* Global JavaScript Objects
  
Each provides useful methods to help interact and manipulate date within the Objects.

  * BOM references: `window.location()`, `window.document()` there are many more. [MDN Refernce](https://developer.mozilla.org/en-US/docs/Web/API/Window)
  * DOM references: `document.createElement()`, `document.querySelector()`: [MDN Reference](https://developer.mozilla.org/en-US/docs/Web/API/Document)
  * Global Objects
    * String: `substring()`, `indexOf()`, `trim()`, 
    * Number: `isNaN()`, `toPercesion()`,
    * Math: `Math.ceil()`, `Math.floor`,
    * Date: `getDay()`, `getFullYear`,
  For more information on the complete list I have provided a link below. There are many more!
    [MDN Reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects)


[Back to TOC](README.md)