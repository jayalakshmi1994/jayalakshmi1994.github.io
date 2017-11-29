## Website Performance Optimization portfolio project
Project Overview:
  
	* The task was to ompitimize the given website with number of optimization and perormance related issues.
	* The page speed for the site has to be increased.
Project Demo
------------	
View the Initial Project : (https://github.com/udacity/frontend-nanodegree-mobile-portfolio)

View the Optimized Project : [Website Optimization](https://jayalakshmi1994.github.io/)


#### PageSpeed Insights

Page speed after optimization

* Desktop 97/100
* Mobile 95/100


A)Tools used for optimization:

* Grunt JS: The Javascript task runner.
* CSS Minifier: Used to minify css.
* JS Compress: To compress the javascript files.
* Kraken.io: To compress the images.



B) Part 1: Optimize `index.html`

** Optimize images
------------------
	* Optimized Images in the index.html to acheive high page speed.
  
** Optimize Render blocking request
-----------------------------------
	* The css files are inlined and  added a media type for ‘print.css’ and added an async tag to the perfmatters.js file.
	 
	<link href="css/print.css" rel="stylesheet" media="print">
    
    <script async src="js/perfmatters.js"></script>


C) Part 2: Optimize `pizza.html`

* Optimized Images in the pizza.html file.
* Recorded timeline traces to find the frame rate.
* In UpdatePosition() function and in the  changePizzaSizes() function the 'querySelectorAll' is changed to 'getElementsByClassName' and querySelector() is changed to to getElementById().

D) Part 3: Measure

* Page speed can be measured at :https://developers.google.com/speed/pagespeed/insights/
* Developer tool is used for further measurements. 