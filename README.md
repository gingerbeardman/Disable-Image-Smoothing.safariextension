# Disable-Image-Smoothing.safariextension
Disables image smoothing using CSS so you can see the individual pixels.

Images that have been affected have a thick red bottom border.

# How?
```css
body > img:only-of-type, .mw-mmv-image img {
	image-rendering: optimizeSpeed !important;
	border-bottom: 4px solid red !important;
}
```

# Which images?
Currently only two types of images are targeted:

* images opened in a new tab or window (images viewed in browser)
* images being viewed using the Wikipedia Media Viewer

If you have any requests for other types of images to include please file a pull request or issue.

# Changelog
2015-01-26, 2.0: Initial Public Version  
2015-01-24, 1.0: Initial Version
