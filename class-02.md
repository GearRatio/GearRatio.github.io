# Duckett HTML & CSS Chapters 2, 10, & 4

## Text
HTML requires both structural and semantic markup. Structural is for the basic foundation of the webpage and semantic provides additional information about the subject matter.

>Semantic HTML is the use of HTML markup to reinforce the semantics, or meaning, of the information in webpages and web applications rather than merely to define its presentation or look. Semantic HTML is processed by traditional web browsers as well as by many other user agents. CSS is used to suggest its presentation to human users.
[Wikipedia](https://en.wikipedia.org/wiki/Semantic_HTML)

Some of the common tags used for the semantic use are:

```
<article>, <aside>, <main>, <figure>, <summary>, <address>, <cite>, <blockquote>, <q>, <abbr>, <ins>, <del>
```

Other tags help to provide emphasis or apply a typographical element. A reference to some of these kind of elements can be found here. [MDN Web Docs HTML Elements Reference](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)

When building out a website it is important to take these elements into consideration and apply them as needed to more accurately apply necessary information.
 
## Introducing CSS
Cascading Style Sheet, or (CSS), allows rules to determine how an element should appear. CSS is a power tool that helps apply aesthetic appeal to many webpages. For smaller pages it can be applied as part of the _in-line_ script or it can be _linked_ as separate files.

_Example External Link_

```
<link rel="stylesheet" href="styles.css">
```
Some webpages will have several CSS Style Sheets. This helps with over maintainability by breaking up the CSS into applied sections.

CSS provides style rules with HTML elements and affects how they are displayed. This is done by using CSS selectors and by then applying a property and value. The property and value make up the declaration and determine how the element should be styled when the rule is applied.

There are several selectors and a reference to them can be found at [MDN CSS Selectors](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Selectors).

CSS has cascading rules that are worth noting. If two or more rules apply to the same element the later will apply. If a rule is more specific than another, the more specific rule will apply. Lastly, if a rule is deemed more _important_ than another then you can add *!important* after the rule. This helps ensure the value should be considered first if any other rules are applied.

Inheritance is another important area of consideration when working with CSS. Some CSS property values set on parent elements are inherited by the children, while some are not. There are  four universal property values for controlling inheritance. They are *inherit, initial, unset, and revert.* Please see, [MDN Cascade and inheritance](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Cascade_and_inheritance).

## Basic JavaScript Instructions
JavaScript is a scripting language that is written in *camelCase*. The first letter fo the word is lowercase while subsequent words are generally uppercase. It is case sensitive.

Statements are organized into code blocks. Some of these statements are surrounded by *{curly braces}*. Closing braces are not followed by a semicolon.

Comments are made using the following methods.
```
//single line comment
/*This is for multi-line comments
and need to be followed with 
the closing use of the asterix
forward slash*/
```

Variables are essential to JavaScript and are used to simply store bits of information for use within the script. Declaring a variable is rather simple. However six rules apply when declaring them.

1. Name must begin with a letter, $, or (_) underscore.
2. Name can't contain (-) or (.).
3. You can't use reserved or keywords [MDN Lexical grammer](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Lexical_grammar)
4. Never create two variables with the same name but different case.
5. Use a name that describes the kind of information being stored.
6. Use *camelCase* if name is made up of two or more words.

```
var overallHeight = 5.10;
let firstName = 'Tim';
const eyeColor = 'blue';
```
Arrays are a kind of list that help to store information. An array can created similarly to how a variable would be created.

```
var myArray = ["Ford", "Chevy", "Honda", "Audi", "Porsche"]
```
Information in array's is accessed via bracket notation. For example, if I wanted to access "Honda" in the array, I would use *myArray[2]*. Array's are zero indexed. This means that first item in the array starts at the number 0 and the 3rd item in the array starts at 2.

You can determine an array's length by calling using the *.length* property. For example, using *myArray.length* will provide the total number of items within the array. This is useful when larger arrays are used.

Information stored in arrays can be updated or changed as needed. For example, myArray[2] = "Tesla" would replace Honda with Tesla.

JavaScript uses expressions to evaluate and return results into a single value. This is done by using operators. These operator are assignment, arithmetic, string, comparison, or logical.

When using arithmetic operators there is a specific order of operation. Multiplication and division are preformed before addition and subtraction. Therefore, it is important to use *parentheses* you want done first inside them. Expressions rely on operators to calculate the value.

Comparison operators allow expressions to determine if the expression is true or false. This is called a *boolean*. A list of these operators can be found at [MDN Expressions and Operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#comparison_operators).


## Decisions and Loops
When creating a script it is  important to determine the behavior of the program based on user interaction. Behavior is created by using evaluations, decisions, and loops.

When evaluating behavior you can create flow charts that breakdown the steps. Another option is to write psuedo code. By breaking down each step into bite size pieces one can take small steps to begin to build out the script.

The use of comparison operators is essential to allowing the evaluation to occur. These operators referenced above help to determine the flow of information as the computer is evaluating it. Operands within the expression do not need to be a single value, ```((x + y) > (a + b)).```

Logical operators allow you to compare the results of more than one comparison. For example, ```((4 > 3) && (5<6))``` evaluates to **true**.

**If** statements check the conditions and determines if it is *true*. If the statement evaluates to true then the rest of the code block runs.

Evaluations lead to decisions. The expression is evaluated, returning a result, then a conditional statement says what to do in a given situation.

```
if(money > 10) {
  console.log("You might be rich!");
} else {
  console.log("You should save your pennies!");
}

```

In the above example, in order for the entire block to execute the fist expression must evaluate too false. The result would return *"You should save your pennies!"*.

[Back to TOC](/Users/jboss/GearRatio.github.io/README.md)