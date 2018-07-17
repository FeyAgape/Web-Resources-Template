# Lity 

[Website](https://sorgalla.com/lity/)

## Lity is a ultra-lightweight, accessible and responsive lightbox plugin which supports images, iframes and inline content out of the box.


## Installation
Include the Lity javascript and css files and its dependencies in your HTML document:
`<head>`
`<link href="lity.css" rel="stylesheet">`
`<link href="prism.css" rel="stylesheet" type="text/css">`
`</head>`
`<body>`


`<script src="jquery.js"></script>`
`<script src="lity.js"></script>`
`<script type="text/javascript" src="prism.js"></script>`
`</body>`

## Usage
Declarative
Add the `data-lity` attribute to <a> elements for which you want the links to be opened in a lightbox:

`<a href="https://farm9.staticflickr.com/8642/16455005578_0fdfc6c3da_b.jpg" data-lity data-lity-desc="Photo of a flower">Image</a>
<a href="#inline" data-lity>Inline</a>
<a href="//www.youtube.com/watch?v=XSGBVzeBUbk" data-lity>iFrame Youtube</a>
<a href="//vimeo.com/1084537" data-lity>iFrame Vimeo</a>
<a href="//maps.google.com/maps?q=1600+Amphitheatre+Parkway,+Mountain+View,+CA" data-lity>Google Maps</a>`

`<div id="inline" style="background:#fff" class="lity-hide">
Inline content
</div>`

If you want to open another URI than defined in the href attribute, just add a data-lity-target with the URI:

`<a href="/image.html" data-lity data-lity-target="/image-preview.jpg">Image</a>`

## Programmatic
Use the global lity function to open URLs (or HTML) in a lightbox or as an event handler.

// Open a URL in a lightbox
var lightbox = lity('//www.youtube.com/watch?v=XSGBVzeBUbk');

// Bind as an event handler
$(document).on('click', '[data-lightbox]', lity);
If you want to close the opened lightbox, use lightbox.close().