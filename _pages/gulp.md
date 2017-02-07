---
ID: 223
post_title: Gulp Install
author: Jeremy Englert
post_date: 2015-06-01 07:49:29
post_excerpt: ""
layout: page
permalink: http://jointswp.com/docs/gulp/
published: true
dsq_thread_id:
  - 'a:1:{i:0;s:10:"3848423070";}'
mashsb_timestamp:
  - 'a:1:{i:0;s:10:"1440724372";}'
mashsb_shares:
  - 'a:1:{i:0;s:1:"0";}'
mashsb_jsonshares:
  - 'a:1:{i:0;s:42:"{"total":0,"facebook_total":0,"twitter":0}";}'
---
Although Gulp is not required to use this theme, JointsWP does come with a <code>gulpfile.js</code>, making it extremely easy to get up and running quickly.

While "the best" way to use the theme is the way that works best for you, using Gulp is definitely the workflow I recommend to get the most out of the theme.
<h3>Getting Started</h3>
<ol>
	<li><a href="https://nodejs.org/" target="_blank">Install node.js</a></li>
	<li>Using the command line, navigate to your theme directory</li>
	<li>Run <code>npm install</code></li>
	<li>Run <code>gulp</code> to confirm everything is working</li>
</ol>
Note: If you run into issues, try installing Gulp globally by running <code>npm install gulp -g</code>.

<hr />

<h3>Gulp Tasks</h3>
<h4>Watching Files for Changes</h4>
Running <code>gulp watch</code> will watch your <code>assets/js/scripts</code> and <code>assets/sass</code> directories for any changes and automatically run the related tasks.
<h4>Compiling Sass</h4>
Running <code>gulp styles</code> will compile all of your Sass files from your <code>assets/sass</code> directory into the <code>assets/css</code> directory. It will create a minified and non-minified file - by default, the theme will enqueue the non-minified file.
<h4>Compiling Custom JavaScript</h4>
Running <code>gulp site-js</code> will combine all of your custom (non-Foundation) JavaScript files from your <code>assets/js/scripts</code> directory into one file in the <code>assets/js</code> directory.

Running this task will create a minified and non-minified file - by default, the theme will enqueue the non-minified file.
<h4>Compiling Foundation</h4>
Running <code>gulp foundation-js</code> will compile all of your Foundation JavaScript files from your <code>vendor/foundation/js/</code> directory into the <code>assets/js/min</code> directory. It will create a minified and non-minified file - by default, the theme will enqueue the minified file.

The <code>gulpfile.js</code> allows you to easily select which Foundation files you want to use. By default all Foundation components are loaded.

[js]

gulp.task('foundation-js', function() {
  return gulp.src([	
  		  
  		  // Foundation core - needed if you want to use any of the components below
          './vendor/foundation-sites/js/foundation.core.js',
          './vendor/foundation-sites/js/foundation.util.*.js',
          
          // Pick the components you need in your project
          './vendor/foundation-sites/js/foundation.abide.js',
          './vendor/foundation-sites/js/foundation.accordion.js',
          './vendor/foundation-sites/js/foundation.accordionMenu.js',
          './vendor/foundation-sites/js/foundation.drilldown.js',
          './vendor/foundation-sites/js/foundation.dropdown.js',
          './vendor/foundation-sites/js/foundation.dropdownMenu.js',
          './vendor/foundation-sites/js/foundation.equalizer.js',
          './vendor/foundation-sites/js/foundation.interchange.js',
          './vendor/foundation-sites/js/foundation.magellan.js',
          './vendor/foundation-sites/js/foundation.offcanvas.js',
          './vendor/foundation-sites/js/foundation.orbit.js',
          './vendor/foundation-sites/js/foundation.responsiveMenu.js',
          './vendor/foundation-sites/js/foundation.responsiveToggle.js',
          './vendor/foundation-sites/js/foundation.reveal.js',
          './vendor/foundation-sites/js/foundation.slider.js',
          './vendor/foundation-sites/js/foundation.sticky.js',
          './vendor/foundation-sites/js/foundation.tabs.js',
          './vendor/foundation-sites/js/foundation.toggler.js',
          './vendor/foundation-sites/js/foundation.tooltip.js',
  ])
[/js]