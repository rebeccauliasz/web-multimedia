---
title: 'CSS3'
date: "2019-09-09"
outputs: "Remark"

cover_img: "css3.jpg" # same dir as slideshow

# remarkJS parameters
ratio: "16:9" #"4:3"
themes:
- apron
- descartes
- adirondack

highlight_style: "atom-one-dark"

---

class: title, smokescreen, shelf, no-footer
background-image: url(css3.jpg)

# CSS3
### Cascading Style Sheets<br />September 9, 2019

---
background-image: url(css3.jpg)

# Review

--
* ### Selectors

---
class: compact

# Selectors

* Are used to _select_ elements of the DOM for styling
--

* Simple selectors:
    * **Universal** - selects all HTML elements&colon; ` * `<br><br>
    * **Type** - selects all HTML elements of a specified type (e.g. `h1`)<br><br>
    * **Class** - selects all HTML elements with the same `class` attribute.  Can be prefixed to select only specific HTML elements with that class (e.g. `.leader` vs `p.leader`)<br><br>
    * **ID** - selects an element with a specific `id` attribute (e.g. `#special`)
--

* High degree of specificity [[CSS Selector Reference](https://www.w3schools.com/cssref/css_selectors.asp)]

---
class: col-2 compact

# Selectors

```html

<body>
    <h1>Title</h1>
    <h2 class="red">Subtitle</h2>
    <p id="special" class="red">Paragraph 1<p>
    <p class="red">Paragraph 2</p>
    <h2>Another Subtitle</h2>
    <p>Paragraph 3</p>
    <p>Paragraph 4</p>
</body>
```

What selector do I use to target:

* All of the elements with the "red" class?
* The element with an ID of "special"?
* The paragraphs with the "red" class?
* The paragraphs that do NOT have a "red" class?
* Paragraph 3?

---
background-image: url(css3.jpg)

# Review

* ### Selectors
--

* ### Cascade

---
class: compact 
# Cascade

The **cascade** is an algorithm that defines how to combine CSS property values originating from different sources, and, when they conflict, determines which has precedent.

* Origin (1 takes highest precedence)
    1. [User Style Sheet](https://davidwalsh.name/firefox-user-stylesheet) (customized by individual users)
    2. Author Style Sheets (Web Designer)
    3. User-Agent Style Sheets (Browser Default)

--
* Page Flow Hierarchy
    * External CSS `<link>` is overridden by 
    * Head CSS `<style>` is overridden by
    * Inline CSS attributes `style=""`

---
class: title

# CSS Layout
## https://learnlayout.com/