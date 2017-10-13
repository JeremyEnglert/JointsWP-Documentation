---
ID: 107
post_title: Getting Started
author: Jeremy Englert
post_excerpt: ""
layout: page
permalink: http://jointswp.com/docs/
published: true
post_date: 2015-01-17 05:59:16
---
<h3 class="alert-box">About These Docs</h3>
JointsWP is a blank WordPress theme built that includes all of the power of <a href="http://foundation.zurb.com/" target="_blank" rel="noopener">Foundation 6</a>. To learn more about specific Foundation components, check out the <a href="http://foundation.zurb.com/sites/docs/" target="_blank" rel="noopener">Foundation 6 Documentation</a>.

The documentation laid out on this site will cover how to get started with JointsWP and how some Foundation components, such as off-canvas components and menus, are integrated with WordPress.

<hr />

<h3>JointsWP Requirements</h3>
JointsWP (Sass version) requires <a href="https://nodejs.org/">Node.js</a> v6.9.x or newer. This doesn't mean you need to understand Node (or even Gulp) - it's just the steps we need to take to make sure all of our development tools are installed.

<hr />

<h3>Download JointsWP and install dependencies with npm</h3>
<div class="highlight highlight-source-shell">

[code]&lt;/pre&gt;
$ cd /wp-content/themes/
$ git clone https://github.com/JeremyEnglert/JointsWP.git
$ cd JointsWP $ npm install

[/code]


At this point, JointsWP should be installed and fully running on your local machine. If you prefer to install the theme manually, that will work as well - just be sure to run <code>npm install</code> after manually moving the files into the <code>/themes/</code>directory.

</div>