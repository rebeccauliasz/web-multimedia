---
title: 'Introduction to Javascript II'
date: "2019-11-11"
outputs: "Remark"

cover_img: "../2019-11-04/javascript.jpg" # same dir as slideshow

# remarkJS parameters
ratio: "16:9" #"4:3"
themes:
- apron
- descartes
- adirondack

highlight_style: "atom-one-dark"

---

class: title, smokescreen, shelf, no-footer
background-image: url(../2019-11-04/javascript.jpg)

# Introduction to Javascript II
## November 11, 2019

---
class: roomy
# Javascript Math Operations

* Addition: `+`:  `let x = y + 1;`<br><br>
* Subtraction: `-`: `let y = 5 - x;`<br><br>
* Multiplication: `*`: `let z = x * y;`<br><br>
* Division: `/`:  `let a = 1 / x;`

---
class: col-2
# Javascript Math Operations, cont'd
<br><br>
* Increment: `++`
* Decrement: `--`;

<br><br>
```javascript
let hitcount = 34;
hitcount++; // 35
hitcount++; // 36
hitcount--; // 35
```
---
# Javascript Assignment Operations, cont'd

| **Operator** | **Example** | **Same As** |
|----------|---------|-----------|
| =        | x = 5;   | x = 5;     |
| +=       | x += 5; | x = x + 5; |
| -=       | x -= 5; | x = x - 5; |
| *=       | x *= 5;  | x = x * 5; |
| /=       | x /= 5;  | x = x / 5; |
| %=       | x %= 5;  | x = x % 5; |


---

# Javascript Functions

---

# Examples

* [Counter](https://jsbin.com/sakimos/edit?html,js,output)


---
# Javascript Array Operations

Get values from arrays using array indexes

```javascript
let a = ["milk", "eggs", "butter"];
let firstItem = a[0]; // milk
console.log(a[1]); // eggs
```
Remember, in most programming paradigms, index numbering begins with `0`

---
# Javascript Array Operations, cont'd

Set values of arrays using array indexes
```javascript
let a = ["eggs","oil","sugar"]
a[3] = "butter"; 
console.log(a); // ["eggs","oil","sugar", "butter"]
```

---

# Javascript Array Operations, cont'd

Replace values from arrays using array indexes
```javascript
let a = ["eggs","oil","sugar"]
a[1] = "butter"; 
console.log(a); // ["eggs","butter","sugar"]
```

---
# Array methods

* sort()
* push()
* pop()
* shift()
* unshift()

---
class: compact
# Logic

if

```javascript
if (condition) {
    // thing to do if true
}
```

if else

```javascript
if (condition) {
  //  thing to do if true
} else {
  //  thing to do if false
}
```
---
class: compact
# Logic

else if

```javascript
if (condition1) {
  //  thing to do if condition1 is true
} else if (condition2) {
  //  thing to do if condition1 is false but condition2 is true
} else {
  // thing to do if both condition1 and condition2 are false
}
```

---
class: compact
# Logic

switch

```javascript
switch(expression) {
  case x:
    // code block
    break;
  case y:
    // code block
    break;
  default:
    // code block
} 
```

---

Putting it all together example:<br>
[https://jsbin.com/buwixeq/edit?html,js,output](https://jsbin.com/buwixeq/edit?html,js,output)

---

# Iteration:  For Loops

Example:  a standard syntax

```javascript
for (statement 1; statement 2; statement 3) {
  // code block to be executed
}
```

Statement 1 is executed (one time) before the execution of the code block.

Statement 2 defines the condition for executing the code block.

Statement 3 is executed (every time) after the code block has been executed.

---

# Iteration:  For Loops

The `for` loop has the following syntax:

```javascript
for (var i = 0; i < 5; i++) {
  // code block to be executed
  alert("All work and no play makes Jack a dull boy.");
}
```

---