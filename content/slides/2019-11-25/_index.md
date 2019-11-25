---
title: 'Fetching Data with Javascript'
date: "2019-11-25"
outputs: "Remark"

cover_img: "json-logo.png" # same dir as slideshow

# remarkJS parameters
ratio: "16:9" #"4:3"
themes:
- apron
- descartes
- adirondack

highlight_style: "atom-one-dark"

---

class: title, smokescreen, shelf, no-footer
background-image: url(json-logo.png)

# Fetching Data with Javascript
## November 25, 2019

---

#  Frontend vs. Backend

* This course has focused on **"frontend"** approaches to web development:

  * Languages:  HTML, CSS, Javascript<br><br>
  * Code is written to run in a web _browser_ (client-side)

--

* **Backend** approaches

  * Languages:  Java, PHP, Python, Ruby on Rails, .Net, Javascript (NodeJS), etc

  * Code is written to run on a web _server_ (server-side) and often interfaces with a _database._

---
class: compact
# Fullstack Development

* "Fullstack" encompasses both front-end (client-side) and back-end (server-side) programming. In addition to mastering HTML and CSS, he/she/they also knows how to:

  * Program a browser (like using JavaScript, jQuery, Angular, or Vue)
  * Program a server (like using PHP, ASP, Python, or Node)
  * Program a database (like using SQL, SQLite, or MongoDB)

--
* Popular full-stack implementations include (in addition to HTML/CSS/Javascript):

    * [LAMP stack](https://en.wikipedia.org/wiki/LAMP_(software_bundle)): Linux - Apache - MySQL - PHP
    * [LEMP stack](https://lemp.io/): Linux - Nginx - MySQL - PHP
    * [MEAN stack](http://meanjs.org/): MongoDB - Express - AngularJS - Node.js
    * [MERN stack](https://medium.com/javascript-in-plain-english/full-stack-mongodb-react-node-js-express-js-in-one-simple-app-6cc8ed6de274): MongoDB - Express - React - Node.js
    * [Python stack](https://www.fullstackpython.com/): Python - Django/Flask/etc - MySQL
    * [Ruby on Rails](https://rubyonrails.org/): JavaScript - Ruby - SQLite - PHP

---
class: compact
# JSON

What is JSON?

--

JSON stands for **J**ava**S**cript **O**bject **N**otation.

--

It is a standard **text-based** format for representing **structured data** based on JavaScript object syntax. It is commonly used for transmitting data in web applications.

---
class: compact 

# Example:   [Who's in Space Right Now?](http://api.open-notify.org/astros.json)

```json
{
    "people": [{
        "name": "Christina Koch",
        "craft": "ISS"
    }, {
        "name": "Alexander Skvortsov",
        "craft": "ISS"
    }, {
        "name": "Luca Parmitano",
        "craft": "ISS"
    }, {
        "name": "Jessica Meir",
        "craft": "ISS"
    }],
    "number": 4,
    "message": "success"
}


```

---

# JSON Formatting

* JSON is purely a data format — it contains only properties, no methods.<br><br>

--
* JSON requires double quotes to be used around strings and property names. Single quotes are not valid.<br><br>

--
* Unlike in JavaScript code in which object properties may be unquoted, in JSON only quoted strings may be used as properties.

---

# Dummy JSON API for testing

* https://jsonplaceholder.typicode.com/

---

# Common Browser APIs

* DOM API
* Fetch API
* Canvas API
* WebGL API
* Web Audio API
* getUserMedia / Stream API
* Device APIs (Ambient Light, Battery, Bluetooth, Vibration)
* Web Storage API

---

# In-Depth:  Getting JSON with the Fetch API

## Generic Fetch Syntax

```javascript
// Replace ./data.json with your JSON feed
// Can be full path URL
fetch('./data.json')
  .then(response => {
    return response.json()
  })
  .then(data => {
    // Work with JSON data here
    console.log(data)
  })
  .catch(err => {
    // Do something for an error here
  })

```

---

# Example 1

[https://jsbin.com/qugosiw/2/edit?html,js,output](https://jsbin.com/qugosiw/2/edit?html,js,output)


---

# Example 2

Parsing this data: [https://jsonplaceholder.typicode.com/users](https://jsonplaceholder.typicode.com/users)

[https://jsbin.com/qugosiw/4/edit?html,js](https://jsbin.com/qugosiw/4/edit?html,js)

---

# Where to look for JSON data:

* https://github.com/public-apis/public-apis
* https://www.data.gov/developers/apis
* https://any-api.com/
* https://www.diycode.cc/projects/toddmotto/public-apis 
