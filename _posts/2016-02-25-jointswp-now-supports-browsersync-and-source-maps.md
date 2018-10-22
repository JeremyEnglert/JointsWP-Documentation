---
ID: 377
post_title: >
  JointsWP Now Supports Browsersync and
  Source Maps
author: Jeremy Englert
post_excerpt: ""
layout: post
permalink: >
  http://jointswp.com/jointswp-now-supports-browsersync-and-source-maps/
published: true
post_date: 2016-02-25 23:10:46
---
Since JointsWP added Gulp, two of the most requested features have been the integration of <a href="https://www.browsersync.io/" target="_blank">Browsersync</a> and Source Maps - I'm happy to say these have been added to the newest version of JointsWP that was released today.

<!--more-->

For those unfamiliar with these two tools, here's a brief overview.
<h2>Browsersync</h2>
If you're familiar with Gulp, you're probably familiar with <code>watch</code> tasks - Browsersync takes <code>watch</code> tasks to the next level.

Whenever you make a change to any of your SCSS files, the change will automatically be injected into all of your browsers - no page reload needed! If you make a JavaScript or PHP change, the browser windows will automatically reload for you.

The GIF below shows a change being made to the settings.scss file, which is then compiled and automatically injected into Chrome (left) and Firefox (right).

<a href="http://jointswp.com/wp-content/uploads/2016/02/jointswp-browsersync.gif" rel="attachment wp-att-379"><img class="aligncenter size-full wp-image-379" src="http://jointswp.com/wp-content/uploads/2016/02/jointswp-browsersync.gif" alt="jointswp-browsersync" width="1658" height="561" /></a>

Getting started with Browsersync is extremely easy. Simply open up your <code>gulpefile.js</code> and look for the Browsersync task (it's near the bottom). Update the "proxy" URL so it matches the URL of your local development enviroment. Now run <code>gulp browsersync</code> from your terminal and enjoy!
<h2>Source Maps</h2>
Concatenating and minifying files is great for performance, however, it becomes a real headache when trying to debug issues as it's no longer easy to tell which file is causing the issue - this is where Source Maps come into play. Source maps allow you to "map" your minified files back to their original, pre-minified state. So when you open up Developer Tools, instead of seeing the minified files, you will see the original source files.

<a href="http://jointswp.com/wp-content/uploads/2016/02/jointswp-sourcemaps.jpg" rel="attachment wp-att-381"><img class="aligncenter size-full wp-image-381" src="http://jointswp.com/wp-content/uploads/2016/02/jointswp-sourcemaps.jpg" alt="jointswp-sourcemaps" width="964" height="357" /></a>

Note: Source maps are only created for minified JS and CSS files. Be sure you're enqueuing the minified files if you want to use source maps.

Questions, comments or concerns? Let's chat in the comments.