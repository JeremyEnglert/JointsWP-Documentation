---
ID: 151
post_title: Bower
author: Jeremy Englert
post_date: 2015-02-02 03:34:49
post_excerpt: ""
layout: page
permalink: http://jointswp.com/docs/bower/
published: true
dsq_thread_id:
  - 'a:1:{i:0;s:10:"3848423156";}'
mashsb_timestamp:
  - 'a:1:{i:0;s:10:"1440725373";}'
mashsb_shares:
  - 'a:1:{i:0;s:1:"0";}'
mashsb_jsonshares:
  - 'a:1:{i:0;s:42:"{"total":0,"twitter":0,"facebook_total":0}";}'
---
The Sass version of JointsWP supports Bower, which allows you to update the included libraries (under<span style="font-family: monospace;"> vendor/</span>) with a single command. If you're new to Bower and don't have it installed, see <a href="http://bower.io/">Bower.io</a> for installation instructions.

From the command line, navigate to your main theme directory. Then run: <code>bower update</code>

This will create a bower_components directory with updated versions of all your vendor files.

That's it! You should see bower go through and update your packages to their newest version.
<h3>Using Gulp?</h3>
Simply run <code>gulp bower</code> to update all vendor files. This will create a <code>bower_components</code> directory with updated versions of the vendor files and automatically move these into the <code>vendor/</code> directory.