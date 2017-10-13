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
<div class="highlight highlight-source-shell">

[code]
$ cd /wp-content/themes/
$ git clone https://github.com/JeremyEnglert/JointsWP.git
$ cd JointsWP $ npm install
[/code]

At this point, JointsWP should be installed and fully running on your local machine. If you prefer to install the theme manually, that will work as well - just be sure to run <code>npm install</code> after manually moving the files into the <code>/themes/</code>directory.

<hr />

<h3>Working with JointsWP</h3>
<h4><a id="user-content-watching-for-changes" class="anchor" href="https://github.com/JeremyEnglert/JointsWP/#watching-for-changes" aria-hidden="true"></a>Watching for Changes</h4>
<div>

[code]$ npm run watch[/code]

</div>
<ul>
 	<li>Watches for changes in the <code>assets/styles/scss</code> directory. When a change is made the SCSS files are compiled, concatenated with Foundation files and saved to the <code>/styles</code> directory. Sourcemaps will be created.</li>
 	<li>Watches for changes in the <code>assets/scripts/js</code> directory. When a change is made the JS files are compiled, concatenated with Foundation JS files and saved to the <code>/scripts</code> directory. Sourcemaps will be created.</li>
 	<li>Watches for changes in the <code>assets/images</code> directory. When a change is made the image files are optimized and saved over the original image.</li>
</ul>
<h4><a id="user-content-watching-for-changes-with-browsersync" class="anchor" href="https://github.com/JeremyEnglert/JointsWP/#watching-for-changes-with-browsersync" aria-hidden="true"></a>Watching for Changes with Browsersync</h4>
<div class="highlight highlight-source-shell">


[code]$ npm run browsersync[/code]


</div>
This will watch the same files as <code>npm run watch</code>, but utilizes browsersync for live reloading and style injection. Be sure to update the <code>URL</code> variable in the <code>gulpfile.js</code> to your local install URL.
<h4>Compile and Minify All Theme Assets</h4>
<div class="highlight highlight-source-shell">


[code]$ npm run build[/code]


</div>
Compiles and minifies all scripts and styles.

</div>