<h1 align="center">3D Layer Image Hover Effect</h1>

<h3 align="center">This program implements a simple scheme for implementing a 3D hover effect with overlaying shadows on an object. This screenshot was taken from a design that was developed for a fitness app. Link to the design of this project: <a href="https://www.behance.net/gallery/41483809/Landing-page-of-the-application-PART_2">Behance</a>
</h3>
<p align="center">
  <img src="https://badges.frapsoft.com/os/v1/open-source.svg?v=103" >
</p>
<p align="center">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original-wordmark.svg" title="html" width="50" height="50"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original-wordmark.svg" title="css" width="50" height="50"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/photoshop/photoshop-line.svg" title="photoshop" width="50" height="50"/>
</p>

## The goal of the work
The main goal of this project is to develop an effect that will create a 3D feel and be visually similar to the up and down fading effect.
This effect will show as one of the visualization effects of a product or object in a presentation or project.

## Task statement
<p>A simple experiment with css & html and its possibilities.</p>
<p>A demo implementation of this template can be viewed at this link:<a href="https://heorhiizemlianko.github.io/3D-Layer-Image-Hover-Effect/3dimaje.html"> <b>3D-Effect</b> </a></p>

## Schematic representation of the HTML structure
```
html
├── head
│   ├── meta
│   ├── title
│   └── link
└── body
    ├── div.container
        ├── img
        ├── img
        ├── img
        └── img
```

## Schematic representation of the CSS structure
```
css
├── body
├── .container
├── .container img
├── .container:hover img: ntn-child(4)
├── .container:hover img: ntn-child(3)
├── .container:hover img: ntn-child(2)
└── .container:hover img: ntn-child(1)
```

## Code from the project
- HTML
```html
<!DOCTYPE html>
<html>
<head>
	<meta charset="utf-8">
	<title>3D Layer Image Hover Effect</title>
	<link rel="stylesheet" type="text/css" href="3dimaje.css">
</head>
<body>
	<div class="container">
		<img src="05_Navigation_Menu.jpg">
		<img src="05_Navigation_Menu.jpg">
		<img src="05_Navigation_Menu.jpg">
		<img src="05_Navigation_Menu.jpg">
	</div>
</body>
</html>
```
- CSS
```css
body{
	margin: 0;
	padding: 0;
	height: 100vh;
	display: flex;
	align-items: center;
	justify-content: center;
	width: 100%;
}
.container{
	position: relative;
	width: 250px;
	height: 415px;
	background: rgba(0,0,0,0.1);
	transform: rotate(-30deg) skew(25deg);
	transition: 0.5s;
}
.container img{
	position: absolute;
	width: 100%;
	transition: 0.5s;
}
.container:hover img:nth-child(4){
	transform: translate(120px, -120px);
	opacity: 1;
}
.container:hover img:nth-child(3){
	transform: translate(90px, -90px);
	opacity: .8;
}
.container:hover img:nth-child(2){
	transform: translate(60px, -60px);
	opacity: .6;
}
.container:hover img:nth-child(1){
	transform: translate(30px, -30px);
	opacity: .4;
}
```
