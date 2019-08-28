---
title: 'Introduction / Course Overview'
date: "2019-08-26"
outputs: "Remark"

cover_img: "html_css_books.jpg" # same dir as slideshow

# remarkJS parameters
ratio: "16:9" #"4:3"
themes:
- apron
- descartes
- adirondack

highlight_style: "atom-one-dark"

---
class: title, smokescreen, shelf, no-footer
background-image: url(html_css_books.jpg)

# Fundamentals of Web-Based<br />Multimedia Communication
### <br />August 26, 2019

---
class: title

## Welcome and Introductions

---
class: col-2

# Teaching Team

- Sinan Goknur, sinan.goknur@duke.edu<br /><br />
- Quran Karriem, quran.karriem@duke.edu<br /><br />
- Luke LeGrand, luke.legrand@duke.edu<br /><br />
- [Mark Olson](https://web.archive.org/web/20000815083047/http://www.duke.edu/web/international/), mark.olson@duke.edu<br /><br />
- Sarah Riazati, sarah.riazati@duke.edu<br /><br />
- Augustus Wendell, augustus.wendell@duke.edu

---
class: col-2 fit-h1 compact

# Key Goal: Development for the Modern Web

The modern web is:

* Standards-based<br />[HTML, CSS, ECMAScript(JS)]<br /><br />

--
* Responsive<br />"Write Once...Display Everywhere"<br /><br />

--
* Accessible<br /><br />

--
* Framework- and component-driven<br /><br />

--
* Collaborative<br /><br />

--
* Always changing<br /><br />

---
class: compact 

# Additional Goals:

* Fluency in web delivery of multimedia content:<br />Audio, images, video, animations, interactive experiences<br /><br />
--

* Break free from Squarespace and Wordpress!<br /><br />
--

* Learn _how_ to learn<br /><br />
--

* Leverage the browser as a _forensic tool:_  [CNN Example](https://cnn.com)<br /><br />
--

* Develop skills in distributed collaborative code development<br /><br />
--

* Have fun _while_ crying in frustration over a missing semicolon<br />"These are tears of joy!"<br /><br />

---

# Program or Be Programmed

>_"When human beings acquired language, we learned not just how to listen but how to speak. When we gained literacy, we learned not just how to read but how to write. And as we move into an increasingly digital reality, we must learn not just how to use programs but how to make them. In the emerging highly programmed landscape ahead, you will either create the software or you will be the software._ 

>**It’s really that simple: Program, or be programmed."**

><cite>― Douglas Rushkoff, [Program or Be Programmed: Ten Commands for a Digital Age](https://rushkoff.com/books/program-or-be-programmed/)</cite>

---

# Class "Deliverables"

>During practical experience lab sessions, students develop a **[personal course webpage](http://people.duke.edu/~nag26/)** to display a portfolio of work completed this semester. These websites are instrumental to our real goals: to uncover multimedia communications principles that scale, work across platforms, and adapt as features and functionality inevitably change in this quixotic and rapidly advancing technological space. 
    
>Throughout the semester, weekly lab exercises will build upon skills and capabilities as students progress toward completion of a final [interactive](http://people.duke.edu/~mcg52/final_project/index.html) [multimedia](http://people.duke.edu/~wjh18/final_project/finalproject.html) [website](http://people.duke.edu/~hew18/Final_Project/final.html). Occasional quizzes will test your understanding of foundational concepts.  In addition, a final project proposal, storyboard, and postmortem report are required.

---

# Grades will be based on:

* Attendance, Labs, and Participation: 30%<br />Labs will be due during by the start of the first discussion section, the week _after_ they are assigned.
--

* Quizzes: 5%  
--

* Midterm Project: 25%<br />Due:  5:00 PM, Friday, October 11
--

* Final Project Proposal: 10%
--

* Final Project: 30%<br />Due: 12:00 PM, Wednesday, December 11
--


Labs will be graded on a | &Oslash; | &#10003; | &#10003;+ | basis.
--


A rubric will help guide the development of your midterm and final projects.  

---
class: title

# Core Technologies

---

# HTML

* A "markup" language for the **"content"** of a website<br /><br />
* Conveys semantic meaning (relative importance/unimportance, type of content)<br /><br />
* Should NOT contain design elements (e.g. using tables for layout)


Example:  http://people.duke.edu/~seminars/csszengarden/

---

# CSS

* A "stylesheet" language for the visual presentation of a website<br /><br />
* aka _graphic design_ through code<br /><br />
* Conveys meaning as well - visual signification

Example:  http://www.csszengarden.com/

---

# Javascript

* A "scripting" language designed to dynamically modify the content and/or visual presentation of a website.<br /><br />
* aka _interactivity_

Note:  CSS3 now has some of this functionality

Example: https://danielfvm.itch.io/bubbles 

---

# HTML5 "Boilerplate"

```html
<!DOCTYPE html>
<html>

<head>
    <meta charset="UTF-8">
    <title>Title of the document</title>
</head>

<body>
    Content of the document......
</body>

</html>
```

---
class: col-2 compact

# For Lab #1 this week

## Install on your laptop:

* Brackets - [brackets.io](http://brackets.io/)
* FileZilla - [Use this download link!](https://filezilla-project.org/download.php?show_all=1)
* [Chrome](https://www.google.com/chrome/) and/or [Firefox](https://www.mozilla.org/en-US/firefox/new/)

## View:

* [What is the Internet?](https://www.khanacademy.org/computing/computer-science/internet-intro/internet-works-intro/v/what-is-the-internet) (3:44)
* [Wires, Cables, and WiFi](https://www.khanacademy.org/computing/computer-science/internet-intro/internet-works-intro/v/the-internet-wires-cables-and-wifi) (6:41)
* [IP Addresses and DNS](https://www.khanacademy.org/computing/computer-science/internet-intro/internet-works-intro/v/the-internet-ip-addresses-and-dns) (6:44)
* [Packets, Routers, and Reliability](https://www.khanacademy.org/computing/computer-science/internet-intro/internet-works-intro/v/the-internet-packet-routers-and-reliability) (6:25)
* [HTTP and HTML](https://www.khanacademy.org/computing/computer-science/internet-intro/internet-works-intro/v/the-internet-http-and-html) (7:06)

---

# For Lab #2 this week:

* Read selected chapters from [HTML &amp; CSS Is Hard](https://internetingishard.com/html-and-css/)
    * [Introduction](https://internetingishard.com/html-and-css/) - and while this resource covers the web editor [Atom](https://atom.io/), see if you can't figure out the analogous functionality in [Brackets](http://brackets.io/).
    * [Basic Web Pages](https://internetingishard.com/html-and-css/basic-web-pages/)
    * [Links &amp; Images](https://internetingishard.com/html-and-css/links-and-images/)

* Sign up for the class Piazza forums:<br />http://bit.ly/fall2019-duke-web-piazza