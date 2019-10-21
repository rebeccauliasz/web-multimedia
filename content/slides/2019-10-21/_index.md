---
title: 'HTML5 Media'
date: "2019-10-21"
outputs: "Remark"

cover_img: "html5_media.jpg" # same dir as slideshow

# remarkJS parameters
ratio: "16:9" #"4:3"
themes:
- apron
- descartes
- adirondack

highlight_style: "atom-one-dark"

---

class: title, fogscreen, shelf, no-footer
background-image: url(html5_media.jpg)

# HTML5 Media (and a little Javascript)
## October 21, 2019

---
class: title

# Midterm Websites Postmortem

---
class: title
# Page Load Times

## Google's [Page Speed Insights](https://developers.google.com/speed/pagespeed/insights/)


---
class: roomy
# Image Optimization

* Suggested Reading:<br><q>[Optimizing Images for the Web:  A Practical Guide](https://www.abetterlemonadestand.com/optimizing-images-for-web/)</q>

* Online tool:  [https://squoosh.app/](https://squoosh.app/)

---
class: compact
# Review:  CSS Transitions

```css
.bar {
    color: #000;
    background-color: #fff;
    width: 80px;
    transition: background-color 500ms ease-out 1s, 
        width 1.5s ease-in, transform 500ms ease-out 1s;
}
.bar:hover {
    color: #fff;
    background-color: #000;
    width: 100px;
    transform: rotate(15deg);
}
```
[https://codepen.io/mjvo/pen/abbBMaB](https://codepen.io/mjvo/pen/abbBMaB)

---
class: compact
# Review: CSS Animations
```css
.box {
  width: 20px; height: 20px; background-color: blue;
  animation-name: bowtie;
  animation-duration: 1s;
  animation-iteration-count: infinite;
}
@keyframes bowtie {
    0% { transform: translate(0px, 0px); }
    25% { transform: translate(300px, 200px) }
    50% { transform: translate(300px, 0px) }
    75% { transform: translate(0px, 200px) }
    100% { transform: translate(0px, 0px) }
}
```

[https://codepen.io/mjvo/pen/vYYyPMj](https://codepen.io/mjvo/pen/vYYyPMj)

---
class: title center 
# A little bit of JavaScript

## [https://codepen.io/mjvo/pen/GRRrjxL](https://codepen.io/mjvo/pen/GRRrjxL)

---
class: title

# HTML5 Media

## Audio and Video for the Web

---
class: roomy col-2
# HTML5 Audio

#### Supported Media Types<br><br><br><br>


| File Format | Media Type |
|-------------|------------|
| MP3         | audio/mpeg |
| OGG         | audio/ogg  |
| WAV         | audio/wav  |

---
class: roomy col-2
# HTML5 Audio
## Browser Support<br><br><br><br><br>

| Browser | MP3 | WAV | OGG |
|---------|-----|-----|-----|
| Edge/IE | YES | NO  | NO  |
| Chrome  | YES | YES | YES |
| Firefox | YES | YES | YES |
| Safari  | YES | YES | NO  |
| Opera   | YES | YES | YES |

---
# HTML5 Audio

## Syntax

```html
<audio controls>
    <source src="filename.ogg" type="audio/ogg">
    <source src="filename.mp3" type="audio/mpeg">
Your browser does not support the audio element.
</audio> 
```

## [Example](https://www.w3schools.com/html/html5_audio.asp)
<audio controls>
  <source src="https://www.w3schools.com/html/horse.ogg" type="audio/ogg">
  <source src="https://www.w3schools.com/html/horse.mp3" type="audio/mpeg">
Your browser does not support the audio element.
</audio>

---
class: roomy col-2
# HTML5 Video

#### Supported Media Types<br><br><br><br>

| File Format | Media Type |
|-------------|------------|
| MP4         | video/mp4  |
| WebM        | video/webm |
| Ogg         | video/ogg  |

---
class: roomy col-2
# HTML5 Video
## Browser Support<br><br><br><br><br><br>

| Browser           | MP4                 | WebM | Ogg |
|-------------------|---------------------|------|-----|
| Internet Explorer | YES                 | NO   | NO  |
| Chrome            | YES                 | YES  | YES |
| Firefox           | YES                 | YES  | YES |
| Safari            | YES                 | NO   | NO  |
| Opera             | YES (from Opera 25) | YES  | YES |

---
class: compact col-2
 # HTML5 Video

## Syntax

```html
<video controls>
    <source src="filename.mp4" type="video/mp4">
    <source src="filename.webm" type="video/webm">
Your browser does not support the video element.
</video> 
```

## [Example](https://www.w3schools.com/html/html5_video.asp)
<video controls width="300">
  <source src="https://www.w3schools.com/html/movie.ogg" type="video/ogg">
  <source src="https://www.w3schools.com/html/movie.mp4" type="video/mp4">
Your browser does not support the audio element.
</video>

---

# HTML5 Video

## WebVTT Syntax

```html
  WEBVTT

  00:00.000 --> 00:02.000
  First Subtitle

  00:02.500 --> 00:04.500
  Second Subtitle

  00:05.000 --> 00:07.000
  And so on . . . 
```


