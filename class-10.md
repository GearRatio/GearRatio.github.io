# Debugging

## Cheat Sheet

Debugging
  1. User Chrome Dev Tools or FireFox when working with JavaScript
  2. Learn to read the console and understand the errors
  3. Set break points when needed
     1. Common errors:
        1. Syntax Error (you made a typo)
        2. Error (The error is based on others)
        3. Reference Error (Tried to reference a variable not defined)
        4. TypeError (Unexpected data type)
        5. RangeError (Numbers not in acceptable range)
        6. URIError (encode and decode not used correctly)
        7. EvalError (`eval()` function used incorrectly)
  4. You can implement a few things to handle errors.
     1. Use Try
     2. Use Catch
     3. Use Throw
     4. Use Finally
  5. Use Dev tools to set break points and evaluate the error.
  6. Console messages `console.log()` helps to pinpoint the error message as the program runs
     1. use `console.log` often as you write your scripts
     2. use the keyword `debugger;` in your code to set a breakpoint
  7. If you know your code may fail use section 4 and implement them along the way. See pages 480-485 for tips.

[Back to TOC](README.md)