---
title: 'CSS3 Animations'
date: "2019-10-14"
outputs: "Remark"

cover_img: "animations.png" # same dir as slideshow

# remarkJS parameters
ratio: "16:9" #"4:3"
themes:
- apron
- descartes
- adirondack

highlight_style: "atom-one-dark"

---

class: title, fogscreen, shelf, no-footer
background-image: url(animations.png)

# CSS3 Animations
## October 14, 2019

---
class: roomy
# CSS Transitions

CSS Transitions allows property changes in CSS values to occur _smoothly_ over a _specified duration_.

[https://codepen.io/mjvo/pen/dyyMpXb](https://codepen.io/mjvo/pen/dyyMpXb)

---
# Anatomy of a CSS Transition

* Transformation must be **triggered**<br>(`:hover` or `:focus` pseudo classes for now, until we learn javascript events)

---
class: compact
# Anatomy of a CSS Transition: Properties

* `transition-property:` - [Required] the property you want to transition.<br>([Not all properties are animatable](https://www.quackit.com/css/css3/animations/animatable_properties/))

* `transition-duration:` - [Required] the length of the transition, in seconds or milliseconds 

* `transition-timing-function:` - [Optional defaults to `ease`]<br>ease | linear 
| ease-in | ease-out | ease-in-out | cubic-bezier | steps<br>[See [https://cubic-bezier.com](https://cubic-bezier.com)]

* `transition-delay` - [Optional] the number of seconds to delay the transition before firing, in seconds or milliseconds

---
# Transition Property Shorthand

`transition: property duration delay timing;`

example:  `transition:  width 2s 30ms linear;`

Multiple properties:<br>
`transition: background-color 2s 1s ease-in, width 3s ease-out;`

---
class: title center

# [https://codepen.io/mjvo/pen/NWWNRga](https://codepen.io/mjvo/pen/NWWNRga)

---
# CSS Animation Property

```css
.animated-thing {
    animation: black-to-white 2s linear 1;
}

@keyframes black-to-white {
    from { background: #000;}
    to { background: #fff;}
}

```

---
class: compact 
# CSS Animation Properties

* `animation-name:` - The name of the `@keyframe` block animation you want to use.

* `animation-duration:` - The length of the animation from 0% &rarr; 100% in s/ms.

* `animation-timing-function:` - similar to `transition-timing-function`<br>

* `animation-delay:` - The number of seconds/milliseconds to delay the animation instead of playing right away

* `animation-iteration-count:` [Default: 1] - The number of times the animation should run from 0% &rarr; 100% until it stops.  Can be set to `infinite`
---
class: title center
# [https://codepen.io/mjvo/pen/NWWNdWK](https://codepen.io/mjvo/pen/NWWNdWK)
---

# Complex Physics

Easing Functions Cheat Sheet
[https://easings.net/en](https://easings.net/en)


[https://codepen.io/mjvo/pen/pooyNQv](https://codepen.io/mjvo/pen/pooyNQv)
