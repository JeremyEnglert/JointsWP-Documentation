---
ID: 223
post_title: 'Getting Started &#8211; Sass'
author: Jeremy Englert
post_excerpt: ""
layout: page
permalink: >
  http://jointswp.com/docs/getting-started-sass/
published: true
post_date: 2015-06-01 07:49:29
---
<h3>JointsWP Requirements</h3>
JointsWP requires <a href="https://nodejs.org/">Node.js</a> v6.9.x or newer. This doesn't mean you need to understand Node (or even Gulp) - it's just the steps we need to take to make sure all of our development tools are installed.

<hr />

<h3>Download JointsWP and Install Dependencies with npm</h3>

[code]
$ cd /wp-content/themes/
$ git clone https://github.com/JeremyEnglert/JointsWP.git
$ cd JointsWP 
$ npm install
[/code]

At this point, JointsWP should be installed and fully running on your local machine. If you prefer to install the theme manually, that will work as well - just be sure to run <code>npm install</code> after manually moving the files into the <code>/themes/</code>directory.

<hr />

<h3>Working with JointsWP</h3>
<h4>Watching for Changes</h4>

[code]$ npm run watch[/code]

<ul>
 	<li>Watches for changes in the <code>assets/styles/scss</code> directory. When a change is made the SCSS files are compiled, concatenated with Foundation files and saved to the <code>/styles</code> directory. Sourcemaps will be created.</li>
 	<li>Watches for changes in the <code>assets/scripts/js</code> directory. When a change is made the JS files are compiled, concatenated with Foundation JS files and saved to the <code>/scripts</code> directory. Sourcemaps will be created.</li>
 	<li>Watches for changes in the <code>assets/images</code> directory. When a change is made the image files are optimized and saved over the original image.</li>
</ul>
<h4>Watching for Changes with Browsersync</h4>

[code]$ npm run browsersync[/code]

This will watch the same files as <code>npm run watch</code>, but utilizes browsersync for live reloading and style injection. Be sure to update the <code>URL</code> variable in the <code>gulpfile.js</code> to your local install URL.
<h4>Compile and Minify All Theme Assets</h4>

[code]$ npm run build[/code]

Compiles and minifies all scripts and styles.
<h4>Compile Specific Assets</h4>
<ul>
 	<li><code>$ npm run styles</code> - to compile all SCSS files in the <code>assets/styles/scss</code> directory.</li>
 	<li><code>$ npm run scripts</code> - to compile all JS files in the <code>assets/scripts/js</code> directory.</li>
 	<li><code>$ npm run images</code> - to optimize all image files in the <code>assets/images</code> directory.</li>
</ul>

<hr />

<h3>File Structure - "Where to Put Stuff"</h3>
<h3>Custom Styles</h3>
<ul>
 	<li><code>style.css</code> - this file is never actually loaded, however, this is where you set your theme name and is required by WordPress</li>
 	<li><code>assets/styles/scss/style.scss</code> - import all of your styles here. If you create an additional SCSS file, be sure to import it here.</li>
 	<li><code>assets/styles/scss/_main.scss</code> - place all of your custom styles here.</li>
 	<li><code>assets/styles/scss/_settings.scss</code> - adjust Foundation style settings here.</li>
 	<li><code>assets/styles/scss/login.scss</code> - place custom login styles here. This will generate it's own stylesheet.</li>
</ul>
<h3>Custom Scripts</h3>
<ul>
 	<li><code>assets/scripts/js/</code> - place your custom scripts here. Each .JS file will be compiled and concatenated when the build process is ran.</li>
</ul>
<h3>>Images</h3>
<ul>
 	<li><code>assets/images/</code> - place your theme images here. Each image will be optimized when the build process is ran.</li>
</ul>