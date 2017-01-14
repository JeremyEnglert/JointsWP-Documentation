---
ID: 214
post_title: 'JointsWP 3 is Fully Baked and Ready for <strike>Lunch</strike> Launch'
author: Jeremy Englert
post_date: 2015-06-10 08:03:33
post_excerpt: ""
layout: post
permalink: >
  http://jointswp.com/jointswp-3-foundation-meets-wordpress/
published: true
dsq_thread_id:
  - "3770709898"
mashsb_timestamp:
  - "1484151420"
mashsb_shares:
  - "26"
mashsb_jsonshares:
  - '{"total":26,"twitter":8,"facebook_total":18}'
---
While at first glance the changes may look minor, this is the largest change to JointsWP since it launched in late 2013. Because of this, it has also been the most tested version of JointsWP - being available on GitHub many months prior to its official launch today.

<!--more-->
<h3>File Structure</h3>
The first thing you'll notice is that the file structure has changed in JointsWP 3. In my opinion, the file structure of a theme (especially developer themes) is extremely important and often overlooked.
<ul>
	<li><code>/library</code> is now <code>/assets</code></li>
	<li><code>/partials</code> is now <code>/parts</code></li>
	<li><code>joints.php</code> is gone - it was essentially just a second functions file anyway</li>
	<li>Each function is now its own file, found in the <code>assets/functions</code> directory</li>
	<li>Many of the Sass files have been removed (small.scss, medium.scss, large.scss, etc.)</li>
</ul>
<h3>Gulp Support</h3>
While Gulp is not required, JointsWP 3 comes packaged with Gulp support. There are many benefits to using Gulp including:
<ul>
	<li>Compile and minify your Sass and JS files quickly (even faster than Grunt)</li>
	<li>Concatenate JS files - JointsWP uses Gulp to compile all of your custom scripts into a production ready, minified JS file</li>
	<li>Less bloat - easily remove unused Foundation components from your install</li>
</ul>
If you aren't already using Gulp (or Grunt), I highly recommend you check it out. However, you can still use CodeKit, Compass or whatever you want to compile your files - it's completely up to you.

<em>But seriously, check out Gulp. You won't regret it.</em>
<h3>Improved Grid Archive and Accordion Archive</h3>
While the <a href="http://jointswp.com/demo/category/grid/" target="_blank">Grid Archive</a> and <a href="http://jointswp.com/demo/category/accordion/" target="_blank">Accordion Archive</a> have been packaged into JointsWP for awhile, they were never the easiest features to use - that has been fixed.

Simply use  <code>get_template_part( 'parts/loop', 'archive-grid' );</code> or <code>get_template_part( 'parts/loop', 'archive-accordion' ); </code>to call the archive style of your choice.
<h3>Other Notable Changes</h3>
<ul>
	<li>Translation support turned on by default</li>
	<li>Custom post type feature turned off by default</li>
	<li>Screenshot.png adjusted for HD/Retina devices</li>
	<li>Removed rarely used CSS classes from Sass files</li>
	<li>Fixed many translation issues</li>
</ul>
<h3>What's Coming Next?</h3>
<a href="http://jointswp.com/foundation-6-development-need-know/">Foundation 6 is coming soon</a> and will be integrated into JointsWP when it arrives. Basic customizer support and improved documentation are also on the roadmap.

Love it? Hate it? Let me know below.