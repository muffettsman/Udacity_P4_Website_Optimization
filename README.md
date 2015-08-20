## Website Performance Optimization portfolio project

Optimized the critical rendering path and make this page render as quickly as possible by applying the techniques learned in the [Critical Rendering Path course](https://www.udacity.com/course/ud884).

### Getting started
Clone this portfolio: frontend-nanodegree-mobile-portfolio-master
Run in local browser.

####Part 1: Optimize PageSpeed Insights score for index.html
	Reference Images were resized to page dimensions.
	All referenced CSS and JS were minified / compressed.
	Added inlined css into html pages via methods prescribed by Google Developers
	Made analytics script loading asynchronous
	
####Part 2: Optimize Frames per Second in pizza.html
	modified views/js/main.js until frames per second rate is 60 fps or higher
	Removed un-necessary js calls in for loop
	Created flag to only animate - reflow/repaint when needed.

####Resources
	PageSpeed Insights: https://developers.google.com/speed/pagespeed/insights/
	Optimize CSS Delivery: https://developers.google.com/speed/docs/insights/OptimizeCSSDelivery
	Leaner, Meaner, Faster Animations with requestAnimationFrame: http://www.html5rocks.com/en/tutorials/speed/animations/