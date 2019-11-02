---
title: 'Web Accessibility'
date: "2019-10-28"
outputs: "Remark"

cover_img: "accessibility.png" # same dir as slideshow

# remarkJS parameters
ratio: "16:9" #"4:3"
themes:
- apron
- descartes
- adirondack

highlight_style: "atom-one-dark"

---

class: title, smokescreen, shelf, no-footer
background-image: url(accessibility.png)

# Web Accessibility
## October 28, 2019

---
# Disability

<br><br>
## Medical vs. Social Model

---
class: roomy
<br><br>
# What is Web Accessibility?

--
A site is accessible when its content is available to, and its functionality can be operated by, literally _anyone_. 

---

# What are some problematic assumptions?

* All users can see well (or at all)<br><br>
--

* All users can see color<br><br>
--

* All users can hear well (or at all)<br><br>
--

* All users can operate a keyboard, mouse, and/or touchscreen<br><br>
--

* All users are habituated to left-to-right content organization<br><br>
--

* All users are neurotypical

???
Accessible sites make accommodations for blindness and low vision, deafness and hearing loss, limited movement, speech disabilities, photosensitivity, and combinations of these, as well as for learning disabilities and cognitive limitations.

---

# Web Content Accessibilty Guidelines (WCAG)

* A W3C Recommendation 
* Currently [version 2.1 (05 June 2018)]()

---
class: compact
# POUR

WCAG is organized around four principles often called by the acronym _POUR_:

--
* **Perceivable**: Can users perceive the content? This helps us keep in mind that just because something is perceivable with one sense, such as sight, that doesn't mean that all users can perceive it.

--
* **Operable**: Can users use UI components and navigate the content? For example, [something that requires a hover interaction](https://ianlunn.github.io/Hover/) cannot be operated by someone who can't use a mouse or touch screen.

--
* **Understandable**: Can users understand the content? Can users understand the interface and is it consistent enough to avoid confusion?

--
* **Robust**: Can the content be consumed by a wide variety of user agents (browsers)? Does it work with assistive technology?

---

# WebAIM's WCAG 2 Checklist 

https://webaim.org/standards/wcag/checklist

---

# WAI-ARIA

- Web Accessibility Initiative's Accessible Rich Internet Applications specification (WAI-ARIA, or just ARIA)<br><br>
- provides the ability for developers to specify roles for significant document areas.

```html
<div id="percent-loaded" role="progressbar" aria-valuenow="75" 
     aria-valuemin="0" aria-valuemax="100" />

```

---

# ARIA Landmark Roles

* banner
* navigation
* main
* search
* article
* complementary (equivalent to aside - supporting content for main content)
* contentinfo (Informational child content, such as footnotes, copyrights, links to privacy statement, links to preferences, and so on.)

---
# Skip Navigation Links

???
Sighted people who use their mouse do not have any trouble with pages such as this. They can almost immediately scan over the page and identify where the main content is. In effect, sighted users have a built-in "skip navigation" mechanism: their eyes.

The main content is not usually the first thing on a web page. Keyboard and screen reader users generally must navigate a long list of navigation links, sub-lists of links, corporate icons, site searches, and other elements before ever arriving at the main content. This is particularly difficult for users with some forms of motor disabilities.

Without some sort of system for bypassing the long list of links, some users are at a huge disadvantage. Consider users with no arm movement, who use computers by tapping their heads on a switch or that use a stick in their mouth to press keyboard keys. Requiring users to perform any action perhaps 100s of times before reaching the main content is simply unacceptable.

---

# Content Linearization

* Code flow
* Use of semantic markup and hierarchical headings

** CSS Grid can be used for good or evil here . . . **

---

# Screen Readers

<iframe width="90%" height="90%" src="https://www.youtube.com/embed/QW_dUs9D1oQ" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---
# Low Vision Simulation

## [ChromeVox Lite](http://udacity.github.io/ud891/lesson3-semantics-built-in/02-chromevox-lite/)

???
The ticket parameters you should specify are:

* one way
* to Melbourne
* leaving on 12 October 2017 (10/12/2017)
* returning on 23 October 2017 (10/23/2017)
* window seat
* do not want to receive promotional offers

---
# Dyslexie Font

# [https://www.dyslexiefont.com/](https://www.dyslexiefont.com/)

---
class: compact
# Autism and Web Accessibility

* Navigation and layout should be consistent across the entire site. Performing the same or similar actions on similar user interface elements should produce similar results.<br><br>
* The site should still be usable at larger text sizes and should still function with images and styles disabled. However, images, icons, and graphics that help with comprehension can be included.<br><br>
* Clutter and distractions should be minimized. Style and white space should separate content and direct the user’s attention as appropriate.<br><br>
* The text should be as simple as possible, while providing definitions for any non-standard terms, such as idioms, jargon, and abbreviations and acronyms. Correct grammar and spelling are important.<br><br>
* Users should have as much control as possible over the site’s behavior. Avoid time limits on content or automatic refreshes whenever possible. Provide clear instructions and error messages when filling out forms.


---
# Lab 06

* https://achecker.ca/checker/index.php
* https://wave.webaim.org
* Use Voice-Over (Mac) on a lab machine in Chrome to experience how a low vision person might experience your site.

Evaluate your site against web accessibility guidelines and respond with a few paragraphs about what you woud change in your midterm website to respond to the accessibility report.
