# Forms, Lists, Tables and Events

## Forms
Forms allow users to input all kinds of different information. In fact the web is riddled with forms. Some that only provide information and others that collect it, use it, and provide services. This information is, once collected is sent in name/value pairs. When a users submits a form, the name of each control is sent to the server in this form and collected. Once the server has received the information it is processed via other programming languages and even potentially stored in a database.

Forms have different form controls and they each have a specific purpose for collecting information. Some of these controls are:
*  Input fields
*  Radio Buttons
*  Check boxes
*  Password input
*  Dropdown boxes
*  Submit buttons

These controls live inside the `<form>` tag. Additionally, there are two way two methods used to send forms. The `get` method and the `post` method. The `post` method is considered more secure for sensitive data such as passwords, can be very long, and allows users to submit data to a database for deleting or storing.

When creating a form make sure to use appropriate attributes for the controls. This helps to ensure that the server knows what field it is requesting and what data is inside it. The `type` field should contain the specific control used for the intended user input or action.

## Lists, Tables & Forms
Lists, Tables and Forms have several specific CSS properties to help with design when creating them. These properties, can be of specific use when working on tables for a salmon cookie project. Some of them are text-align, text-transform, and padding, width.

Forms also have some similar properties and can gain visual enhancement with styling using CSS. This information is covered on pages 342 through 347.

In short, forms are powerful tools that, when layed out correctly, can be useful for collecting information. Proper layouts make them feel more interactive.

## Events
Interactions create events and events trigger a program to respond to them and those programs in turn respond to the users interacting with it. Events can be broken down into six catagories. Each category has specific events associated with it.
  * UI events
  * Keyboard events
  * Mouse events
  * Focus events
  * Form events
  * Mutation events

Event handling is when a user interacts with the HTML and it triggers a script to run via JavaScript. There are three steps in order to trigger events. Select the element, specify the event, call the code. These event handlers are usually specified through the DOM or via Event Listeners. Pages 251 thorough 259 go into more details on how to implement some of these events. 

It is important to understand flow and be aware of `Event Bubbling`. In short, by setting an event listener on the innermost child of an element it has an outward affect through the DOM tree. Other event listeners can be placed along parent elements to further handle DOM delegation. This information can be handled via the event object. This type of approach has many benefits and is further explained on pages 268 through 277.

Events help indicate when something has occurred within the browser or window. By binding events to listeners you are able to stat which event occurred, what should happen next, and on which element it should happen. When events happen it can trigger a JavaScript function. This increases user interaction and enhances the overall user experience. The most commonly used are DOM events but others can be specified.

[Back to TOC](README.md)