# Duckett JS Book: Chapters 3 and 5

## Problem Domains
[DZone](https://dzone.com/articles/understanding-problem-domain)
Problem domains are just puzzles that lack all the information. Programmers are not often always given all fo the information to solve the problem. Therefore, by understanding the problem domain, writing code becomes easier. So when the problem is not clear try breaking it down into smaller parts and focus on those first.

Additionally, take time to understand the problem fully before beginning to write code. By ensuring you fully understand the problem, inside and out, should you being to code.

## What's the difference between primitive values and object references in JS?
[betterprogrammingpub](https://betterprogramming.pub/intermediate-javascript-whats-the-difference-between-primitive-values-and-object-references-e863d70677b)

All data types fall into two catagories in JavaScript, primitive values and object references. Each behaves differently and this had a broad affect on how JS functions. Eight data types exist in JS. They are boolean, Null, Undefined, Number, BigInt, String, Symbol, Objects.

When a primitive value is assigned to a variable it's value is set directly to the variable.

When an object is created JavaScript creates the object and stores it in computer memory. The actual value of the variable then hold a reference to the memory address that is currently storing the object.

  * primitive data is immutable, you can get around by reassigning the a new value to the variable
```js
 let word = 'map'
 word = `n${word.slice(1)}
 //console.log(word) // "nap"
```
  * object references are mutable
    * arrays are mutable objects in JavaScript
  * When altering objects it is important to use `Object.assign`
    * it accepts the target object, the properties are assigned.
  
```js
let lead = {
  name: 'John Lennon',
  group: 'The Beatles'
}
let coLead = Object.assign({}, lead, {
  name: 'Paul McCartney'
})
 console.log(lead, coLead)
// {name: "John Lennon", group: "The Beatles"}
// {name: "Paul McCartney", group: "The Beatles"}
```

The above example allows you to copy part of one object from another and still keep the original object unchanged.

Because objects contain references to their location logical operators do not work the same as one would expect. By converting these to primitive data types, it is a little easier to then use comparison operators if needed.

* json.stringfy()
* json.parse()
  [MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/JSON/stringify)

## Object Literals
Objects that hold variables are known as properties and objects that hold `functions` are known as methods. Objects are made of `key` and `value` pairs. Objects can't have identical keys. Each must be unique. You access the object with dot notation or with bracket notation.

You can pass parameters in methods contained in objects if you need.

```js
var hotel = {
name: "hotel jared"
rooms: 45
booked: 18
checkAvailability() {
  return this.rooms - this.booked;
}
}
hotel.checkAvailability() //parameters can be added
```
## Document Object Model
JavaScript can access and update the DOM via accessing methods and properties. A DOM can also be referred to an an Application User Interface or (API). In short, API's let programs and and scrips talk to each other.

The DOM tree is a model of a web page.
  * document (root)
    * html
    * body
    * div
      * attribute (opening tags of html)
    * h1 (element node)
      * attribute (opening tags of html)
    * h2 (element node)
      * text (text nodes)
    * ul (element node)
      * li (element node)
        * attribute (opening tags of html)
      * text (text nodes)
*Scripts access and update the DOM tree (not the HTML source), any changes are reflected in the browser*

You can select individual nodes:
  - getElementById()
  - querySelector()

You can select multiple elements (nodelists)
  - getElementsByClassName()
  - getElementsByTagName()
  - querySelectorAll()

Traverse between element nodes
  - parentNode
  - previousSibling / nextSibling
  - firstChild / lastChild

Access / update text nodes
  - nodeValue

Work with HTML Content add and remove nodes
  - innerHTML
  - textContent
  - createElement()
  - createTextNode()
  - appendChild() / removeChild()

Access or update attribute values
  - className / id
  - hasAttribute(), checks if it exists
  - getAttribute(), gets value
  - setAttribute(), sets its value
  - removeAttribute(), removes an attribute

DOM queries allow you to use methods to find elements in the DOM tree. Use a variable to store is value if you need to access it more than once. Also by storing an element in a  variable you are generally storing the location of that element.

Element nodes are stored, starting at 0, in the order they appear on the HTML page.

NodeLists is numbered like and array and is indexed like an array. They return an `object` and are not actually arrays. Using the `item()` method returns a specific node from the NodeList when you provide it the index number. It is also possible to use `[]notation`.

Using `getElementsById` returns a live node list while `querySelector` returns a static node list.
###  Traversing the DOM
When you have an element Node you can select another element in relation to it using five properties
  - parentNode
  - previousSibling / nextSibling
  - firstChild / last Child

White Space Nodes *some browsers add a text node whenever they come across whitespace between elements.*
  - previousSibling
  - nextSibling
  - firstChild
  - lastChild

`nodeVale`  property of the Node interface returns or sets the value of the current node.

Dom manipulation methods are safer and allow you to use methods to create element and text nodes, then attach them to the tree, or remove them. In order to add content you use a DOM method. This is done one node at a time. You use another DOM method to attach it to the tree.

Getting and updating element contents is done with several other DOM elements. A few of them are listed below.
  - innerHTML() / see pages 226 and 227
  - createElement()
  - createTextNode()
  - appendChild()

## DOM Tools
Browsers such as Chrome and FirFox offer tools to test, examine, and evaluate many of the DOM properties.

[Back to TOC](README.md)