# Duckett HTML & CSS Chapters 4, 15, 3 (Duckett JS Book)

## Links
Links are necessary to understand in order to allow the user to go to other pages contained within the site, or access necessary external sites.

Links are created using `<a>` tags. I have provide an example below.

```html
<a href=http://www.weather.com">Weather</a>

```
When linking to pages within your own site you only need to reference the relative url. However, as shown above, when accessing external sites you should reference the absolute.

Additional, you can specify links to open other windows, target content within your own site, or send an email. For further reading see, you guess it, [MDN Link Types](https://developer.mozilla.org/en-US/docs/Web/HTML/Link_types)

### Directory Structure
When setting up files you should consider following a `tree` format. The `root` folder is where all other files and folder will be stored. Other folders within the root should contain a label that highlights what is contained.

When constructing these folders and sub-folders, any links within the website need to be maintained according to the directory path.

## Layout
Page layout is an important concept to understand. It can also be frustrating. By paying attention to the elements and grouping, you can create page layouts that easy to understand and flow well. I will provide an overview of the following.
  * How to position elements normal flow, relative positioning, absolute and floats
  * Be aware of different screen size requirements
  * Learn key differences between fixed and liquid layout
  * Use of grids to layout a page

When working with block and inline elements it is important to understand how each flow and how CSS treats those HTML elements. CSS treats HTML as if each item is a box. However, inline elements don't act like block elements. In order to better handle them it is a good idea when laying out a page to consider grouping and "containing". See my example below.

```html
  <html>
    <div class="container">
      <nav>
        <ul>
          <li><a href="">Home</a></li>
          <li><a href="">News</a></li>
          <li><a href="">Contact</a></li>
          <li><a href="">About</a></li>
        </ul>
      </nav>
    </div>
</html>

```
The DIV acts as a container element to help group elements together. The **containing** element is always the direct parent of that element.

Controlling items on a page is known as flow. The following allow the editor to choose how the content sits within the page.
  **Normal Flow**
  Every block element appears on a new line and flows top to bottom.
  **Relative Positioning**
  This moves an element from its normal position and shifts it to where the  site editor has chooses to place it. It does not affect its surrounding elements.
  **Absolute Positioning**
  Positions the element in relation to its containing element. It is taken out of normal flow. Absolute position elements move as users scroll up and down the page.
  **Fixed Positioning**
  This positions the element in the browsers window instead of positioning it in relation to the containing element. It is a form of absolute positioning.
  **Floating Elements**
  Floated elements takes the element out of normal flow. Once done those elements become block level elements.
See link for further examples and detailed explanation.
[MDN Position](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Positioning)

## Screen and Page Sizes
When creating a site it is important to design the site using a mobile first approach. This term takes into consideration that many screen sizes and resolutions exists. Luckily, your google dev tools can help you with determining how to begin to approach this problem. Additionally, the book talks about using a liquid layout. It is important to understand the disadvantages of a fixed layout and a liquid layout. Responsive design is mandatory. See [MDN Responsive Design](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Responsive_Design)

One way to assist with screen size changes is the use of a media queries. This allows the developer the ability to control what and how the content is displayed on different sized screens. An example is provided below. Using this approach along with chrome dev tools and testing out the screen sizes helps with CSS control and site development.

```css
@media screen and (min-width: 900px){
  .container {
    margin: 1em 2em;
  }
  }

```

## Grids
So what is a grid?
>A grid is a set of intersecting horizontal and vertical likes defining columns and rows.--source [MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Grid_Layout/Basic_Concepts_of_Grid_Layout)

By approaching page layout in a grid it allows the developer to position items and create a flow and overall structure. Additionally, grids help to
  * provide predictable structure
  * make it easier to maintain
  * allow for greater collaboration
  
These key areas provide a better user experience when done correctly. There are pre-designed grids available. The book recommends [960Grid]((https://960.gs/))

Other frameworks to consider:
  * [JuicedCss](http://juicedcss.com/)
  * [milligram](https://milligram.io/)
  * [blueprintCss](http://blueprintcss.org/)

There are others and I recommend googling and reading the technical documentation to learn more.

Lastly, consider keeping your CSS modular. Doing so has many advantages. Creates less work, only have to update one sheet, reduces confusion, and helps with consistency. You can import fonts, other CSS style sheets by including the `@import` at the **Top** for your CSS file.

## Functions, Methods, and Objects

In JavaScript functions allow you to group a series of statements together to preform certain tasks. This is especially helpful if you need to use the same task over and over. Functions also provide reusable code.

Functions take in parameters, these parameters provide the function with needed information to complete the task.

Functions also take in arguments. Arguments are noted below. The below is also known as declaring a function.

```js
function someName(argumentA, argumentB) {
  //does something with parameters here
  //return parameter;
}

```

Once the function has been defined you can then call it when needed.

```js
//call function
someName(argumentA, argumentB);

```

In order to get a function to return a value you need to make sure that you tell the function to return the information. This isn't always required and depends on the nature of the function.

Variables can also hold function. This is useful and encourages a `DRY` approach. DRY stands for Do Not Repeat Yourself. It simply cuts down on repetitive code and makes the program more readable.

Functions can use `local` and `global` variables. A local variable is a variable declared within the function. A global variable is declared outside the function and can be accessed by other functions.

[Back to TOC](README.md)