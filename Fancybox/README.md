# Fancybox

fancyBox is a tool that offers a nice and elegant way to add zooming functionality for images, html content and multi-media on your webpages. It is built on the top of the popular JavaScript framework jQuery and is both easy to implement and a snap to customize.

[Website](http://fancyapps.com/fancybox/)


## Instructions
Include the files and include fancyBox script and stylesheet in your document (you will need to make sure the css and js files are on your server, and adjust the paths in the script and link tag). Make sure you also load the jQuery library. Example:

`<!-- Add jQuery library -->`

`<script type="text/javascript" src="http://code.jquery.com/jquery-latest.min.js"></script>`

`<!-- Add mousewheel plugin (this is optional) -->`

`<script type="text/javascript" src="/fancybox/lib/jquery.mousewheel-3.0.6.pack.js"></script>`

`<!-- Add fancyBox -->`
`<link rel="stylesheet" href="/fancybox/source/jquery.fancybox.css?v=2.1.7" type="text/css" media="screen" />`

`<script type="text/javascript" src="/fancybox/source/jquery.fancybox.pack.js?v=2.1.7"></script>`

`<!-- Optionally add helpers - button, thumbnail and/or media -->
<link rel="stylesheet" href="/fancybox/source/helpers/jquery.fancybox-buttons.css?v=1.0.5" type="text/css" media="screen" />
<script type="text/javascript" src="/fancybox/source/helpers/jquery.fancybox-buttons.js?v=1.0.5"></script>
<script type="text/javascript" src="/fancybox/source/helpers/jquery.fancybox-media.js?v=1.0.6"></script>
<link rel="stylesheet" href="/fancybox/source/helpers/jquery.fancybox-thumbs.css?v=1.0.7" type="text/css" media="screen" />
<script type="text/javascript" src="/fancybox/source/helpers/jquery.fancybox-thumbs.js?v=1.0.7"></script>`

Create link elements whose href attributes will contain the path of the element you wish to open within the fancyBox.

`<a class="fancybox" rel="group" href="big_image_1.jpg"><img src="small_image_1.jpg" alt="" /></a>
<a class="fancybox" rel="group" href="big_image_2.jpg"><img src="small_image_2.jpg" alt="" /></a>`	

Attach fancyBox when the document is loaded. If you are not familiar with jQuery, please, read this tutorial for beginners.

``<script type="text/javascript">
	$(document).ready(function() {
		$(".fancybox").fancybox();
	});
</script>`