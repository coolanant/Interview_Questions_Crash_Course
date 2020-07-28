# Interview_Questions_Crash_Course

## JavaScript

1. **Event delegation** refers to the process of using event propagation **(bubbling)** to handle events at a higher level in the DOM than the element on which the event originated. It allows us to attach a single event listener for elements that exist now or in the future.

2. An **IIFE** (Immediately Invoked Function Expression)
```javascript
(function() {})();
```
3. **Function Declarations vs. Function Expressions**
Function declarations load before any code is executed 
while Function expressions load only when the interpreter reaches that line of code.
```
ex function bar() {return 3;}
ex var x = function (a, b) {return a * b;}
```

4, **Hoisting**
Hoisting is a JavaScript mechanism where variables and function declarations are moved to the top of their scope before code execution.
Inevitably, this means that no matter where functions and variables are declared, they are moved to the top of their scope regardless of whether their scope is global or local.

ex- 
```
function hoist() {
  a = 20;
  var b = 100;
}

hoist();

console.log(a); 
/* 
Accessible as a global variable outside hoist() function
Output: 20
*/

console.log(b); 
/*
Since it was declared, it is confined to the hoist() function scope.
We can't print it out outside the confines of the hoist() function.
Output: ReferenceError: b is not defined
*/
```
