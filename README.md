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
	@: 409, 412, 415, 427 Updated document.querySelector to document.getElementById - Web API call is faster.
	@: 451, 529 Updated document.querySelector to document.getElementsByClassName - Web API call is faster.
	@: 478 Declared var pizzasDiv outside the for loop so the function only makes one DOM call.
	@: 506 created var lastScrollY to hold last scroll position
	@: 507 created var animateCheck as a flag to animate frame only once per update
	@: 515 created checkFlag() func that checks the status of animateCheck bool and calls requestAnimationFrame if flag is off
	@: 510 created onScroll func bound to scroll window event listener @: 548
	@: 511 sets lastScrollY to current pixels scrolled from top
	@: 512 calls checkFlag func to animate frame once
	@: 525 resets animateCheck flag 
	@: 530 currentScrollY modified to calc from lastScrollY
	@: 533 phase adjusted for the current position
	@: 548 window event listener that triggers onScroll func
	

####Resources
	API References: https://developer.mozilla.org/en-US/docs/Web/API/Document/getElementById
		https://developer.mozilla.org/en-US/docs/Web/API/Document/getElementsByClassName
		https://github.com/udacity/fend-office-hours/tree/master/Web%20Optimization/Effective%20Optimizations%20for%2060%20FPS
	PageSpeed Insights: https://developers.google.com/speed/pagespeed/insights/
	Optimize CSS Delivery: https://developers.google.com/speed/docs/insights/OptimizeCSSDelivery
	Leaner, Meaner, Faster Animations with requestAnimationFrame: http://www.html5rocks.com/en/tutorials/speed/animations/