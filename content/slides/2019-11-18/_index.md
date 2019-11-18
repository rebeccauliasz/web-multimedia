---
title: 'Introduction to Javascript III'
date: "2019-11-18"
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

# Introduction to Javascript III
## November 18, 2019

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
# Javascript Functions

Syntax:

```javascript
function functionName(param1, param2) {
  // do stuff here - example: 
  //let sum = param1 + param2;
  //return sum;
}

```

---
# Javascript Objects

Encapsulated data types that contains properties (variables) and methods (functions).  Objects are declared and then instanced.

---

# Methods for creating objects

* Object Literals
* Constructor Function
* Object.Create method [not covered today]
* ES6 Class

---
class: compact

# Object Literal


```javascript
let car = {
  model: 'Escort', 
  make:'Ford', 
  engine:'4 cylinder'
  start: function(){
      console.log("starting engine");
  }
};

console.log(car.make); // Ford
car.driveType = "4WD"; // set an object property

```

---
class: compact
# Constructor Function

```javascript
function Car(make, model, engine) {
    this.make = make;
    this.model = model;
    this.engine = engine;
    this.start = function(){
      console.log("starting engine");
    }
}

let car1 = new Car('Ford', 'Escort', '4WD');
let car2 = new Car('Honda', 'Civic', 'AWD');

console.log(car2.make); // Honda
car2.start(); // starting engine

```

---
class: compact
# ES6 Class

```javascript
class Car {
    constructor(make, model, engine){
      this.make = make;
      this.model = model;
      this.engine = engine;
    }

    start() {
      console.log("Starting...");
    }
}

let car1 = new Car('Ford', 'Escort', '4WD');

car1.brake = function(){
  console.log("Braking...");
}

car1.brake(); // Braking... 

```

---

# Implementing a Javascript Library

https://tingle.robinparisi.com/

---
# Using a CDN (Content Delivery Network)

https://cdnjs.com/