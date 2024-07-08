# Technical Paper on AMA held on July 6

### 1. What is the difference between ( === ) and ( == ) operator ?
- ( == ) operator is used to compare based on values and ( === ) operator is used to compare on both values and types.

### 2. Console.log(typeof []) is equals to 'object' why?
- typeof [] is object in javascript because it internally stores indices as keys and also supports the methods of objects.

### 3. Whats are the disadvantages of using closure?
- The disadvantage of closure is that garbage collector cannot remove the space allocated by the closure variable.

### 4. Why using global variables are bad in js ?
- Using global variable is a bad practice in javasctipt because sometimes it may lead to naming conflicts and can be very hard to debug.

### 5. How to extract certain properties from an array of objects to create a new array ?
- We can use higher order function like filter to extract values based on the certain condition.


### 6. Difference between charAt() and at() method in js ?
- The main difference between charAt() and at() is that charAt() method returns a empty string when the index out of bound it returns a empty string and with the at() method it returns undefined.

###  7. How to reset initial or 1st commit in git, if its possible ?
- It is not possible to revert the first commit instead of that we can create w new branch and make changes and commit and delete the old one.

### 8. If console.log(typeof []) returns 'object', then why can not we use (.) operator in array to accesss its values just like objects,where we use (.) operator in objects for accessing key and values?
- There are certain differences between the arrays and objects and the main differnece is arrays key is numerical indices and the object keys is in the string form.

### 9. Why 'forEach' loop skips 'not defined' whereas 'for' loop gives 'undefined' ?
- for loops traverse by indexes so when the element will be absent it will be treated as undefined and forEach loops traverses by element to element so it does not  takes care about the absent element.

### 10. How can we mimic the action Array.splice and 'Array.slice' on objcts?
- for mimicing the method for object may requires to create the custom functions and return it explicitly.


### 11. What is "Callback Hell" problem and how to avoid it ?
- callback hell is a situtation where one callback function calls another callback and so on. For avoiding this we can use promises.

### 12. Question:-
let ar = [1,2,3];
console.log("Hello");
module.exports.ar = ar;

// file2.js
const {ar} = require('file1.js');
let print = ar;
console.log(print);

Output: "Hello" 
        [1,2,3]

- why "Hello" is also printing ? when we have exported array('ar') only?

#### Explanation:-
- When we export any module the execution of the module happens regardless of what we imported so all the statement got executed.We may limit this behaviour by making a function and make a call when needed.