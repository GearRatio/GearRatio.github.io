# Summary for chapters 1, 8, 17, 18 & JS Chapter 1

## Structure
Accessibility is important when developing a site. HTML, CSS and JavaScript create layers to a site. Tags provide the structure. Attributes provide definition and can increase function. You can have *several classes* just separate them with a space

```
<html>
    <head>
        <title lang="en-us">Example title with attribute.</title>
    </head>
    <body>
    <!--Start of Main Text-->
        <h1 class="heading underlined">First heading within body</h1>
        <p>Information will be displayed within body tags</p>
    <!--End of Main Text-->
    </body>
</html>
```    
## Extra Markup
HTML5 is the current markup version. It is important to know about older versions and to be aware of browser compatibility issues. "DOCTYPE" indicates the version of HTML.

ID's are global elements but must be unique and can not be used repeatedly but can be used on any element. Classes can be used on any element within html.

Inline elements take up the full line and block elements follow one another on screen.

Div and Span allow you to group block and inline elements together.

Reference: [Mozilla Reference](https://developer.mozilla.org/en-US/docs/Web/HTML/Block-level_elements#block-level_vs._inline)

HTML & CSS Escape Characters: [John Duckett Reference](http://www.htmlandcssbook.com/extras/html-escape-codes/)

## HTML Layout
Creating a basic site structure is important and certain elements should be grouped together. Use semantic markup when laying out the site.

Non-semantic tags can be used when you are not able to properly use a semantic tag. In this case use of div and span are acceptable.

Reference: [Mozilla Layout Reference](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Document_and_website_structure)

## Process & Design
It is important to define, who, why, what, and how, before building a site. A conceptual approach such as wireframing or using simple cards to layout the layers can help with creating the blocks of the site. Take into account visual hierarchy and use size and color to establish a flow for the site. Group similar items in order to simplify.

## JavaScript Summary
JavaScript helps increase user interaction and provides a set of specific instructions to a computer in order to achieve its task.Start designing a script by taking small tasks and breaking each down. Work through each step of the task until completed.

Object can be made of:
 * Properties
 * Events
 * Methods

The above can represent the Document Object Model, DOM, and is the foundation of a website.
 * Document is the root
 * HTML is the trunk
 * Head and Body form branches

JavaScript allows each portion of the DOM to be accessed and manipulated if needed. JavaScript should be kept in a separate file an linked using script.
    
[Back to TOC](GearRatio.github.io)