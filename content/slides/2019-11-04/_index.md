---
title: 'Introduction to Javascript'
date: "2019-11-04"
outputs: "Remark"

cover_img: "javascript.jpg" # same dir as slideshow

# remarkJS parameters
ratio: "16:9" #"4:3"
themes:
- apron
- descartes
- adirondack

highlight_style: "atom-one-dark"

---

class: title, smokescreen, shelf, no-footer
background-image: url(javascript.jpg)

# Introduction to Javascript
## November 4, 2019

---
class: compact
# Core Technologies (Review)

--

* HTML
    * A "markup" language for the **"content"** of a website
    * Conveys semantic meaning (relative importance/unimportance, type of content)

--
* CSS
    * A "stylesheet" language for the visual presentation of a website (incl. animation)
    * aka _graphic design_ through code

--
* **Javascript**
    
    * A "scripting" language designed to dynamically modify the content and/or visual presentation of a website. 
    * aka _interactivity_ / _modifying the DOM_

---
# What is the DOM?

The *Document Object Model* is a cross-platform and language-independent interface that treats an XML or HTML document as a tree structure wherein each node is an object representing a part of the document. The DOM represents a document with _a logical tree_.

![DOM](https://www.w3schools.com/js/pic_htmltree.gif)

---
# What is the DOM?

With the Document Object Model, programmers can build documents, navigate their structure, and add, modify, or delete elements and content. Anything found in an HTML or XML document can be accessed, changed, deleted, or added using the Document Object Model

---
class: compact
# Javascript 101 - Data Types

There are 7 "primitive" data types in Javascript:
--

* **Number** - for numbers of any kind: integer (-1, 24, 0) or floating-point (2.343, 1.0, 3.14159265).<br><br>
--

* **String** - for characters or strings of characters ("m" or "water" or "My name is Sam.")<br><br>
--

* **Boolean** - for `true` or `false`<br><br>
--

* **Null** - a special value which represents “nothing”, “empty”:  `null`<br><br>
--

* **Undefined** -  for unassigned values (e.g. variables declared but not defined: `var x;`)<br><br>
--

* **Object** - for more complex data structures (object-oriented programming)<br><br>
--

* **Symbol** (new in ES6) - tokens that serve as unique IDs

---
# Javascript - Variables

A variable is a “named storage” for data.  Contemporary Javascript programming uses the keyword `let` to declare a variable.


```javascript
let x = 1;
let y = "My first sentence.";
let is_it_on = false;
```

--
Older versions of javascript used the keyword `var`.  

```javascript
var k = 2.354;
```
_(Don't worry about the distinction for now.)_

---
# Javascript - Arrays

An **array** is used to store multiple values in a single variable.

```javascript
let fruits = ["apple", "pear", "banana"];
let ages = [21, 33, 87];
```
--
To access an element in an array, you use its "index."  In most programming paradigms, the first item in an array is index `0`, the second is `1`, the third is `2`, and so on.

```javascript
let favorite = fruits[1];  // returns "pear" from the array above
let disgusting = fruits[0]; // returns "apple"
```

---
class: compact 
# Javascript - Selecting DOM Elements

* The `getElementById()` method:  returns (or "gets") the DOM element that has the ID attribute with the specified value.

    ```javascript
        let myDiv = document.getElementById("div1");
    ```
    
    [getElementById Example](https://jsbin.com/befucax/edit?html,js,output)

--
<hr>

* The `getElementsByTagName` method:  returns (or "gets") the DOM element of the specified element type.  In the code below, it will select all list items `<li>`

    ```javascript
        let myDiv = document.getElementsByTagName("li");
    ```
    [getElementsByTagName Example](https://jsbin.com/vuvuyuy/edit?html,js,output)

---
class: compact
# Javascript - Selecting DOM Elements, cont'd

* The `getElementsByClassName()` method: returns all DOM elements that share a specified class name.

    ```javascript
    let allBirds = document.getElementsByClassName("bird");
    ```
    [getElementsByClassName Example](https://jsbin.com/yasoxov/edit?html,js,output)
--
<hr>
* The `querySelector()` method: returns the _**first**_ DOM element that shares the specified CSS selector.

    ```javascript
    let firstBird = document.querySelector(".bird"); // returns first element with .bird
    let firstPara = document.querySelector("p"); // returns first <p> element
    ```
    [querySelector Example](https://jsbin.com/goyoxor/edit?html,js,output)

---
class: compact
# Javascript - Creating and inserting DOM elements

1. To create a new DOM element, use the `createElement` method:

    ```javascript
    let newElement = document.createElement("p");
    ```

--
1. To add content to that new DOM element, set its `innerText` or `innerHTML` properties:

    ```javascript
    newElement.innerText = "This paragraph created by JS!";
    ```

--
1. Finally, insert the new DOM element into the DOM:

    ```javascript
    document.body.appendChild(newElement);
    ```

---
# Two methods of insertion

1. The **`appendChild()`** method: adds a node to the _end_ of the list of children of a specified parent node.<br><br>syntax: `parentNode.appendChild(newNode);`

--

1.  The **`insertBefore(newNode, beforeNode)`** method: inserts a node before the reference node as a child of a specified parent node.<br><br>syntax: `parentNode.insertBefore(newNode, referenceNode);

---
# Replace Child

https://www.w3schools.com/jsref/met_node_removechild.asp
