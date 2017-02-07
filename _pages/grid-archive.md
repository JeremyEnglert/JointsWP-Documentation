---
ID: 161
post_title: Grid Archive
author: Jeremy Englert
post_date: 2015-02-02 03:50:37
post_excerpt: ""
layout: page
permalink: http://jointswp.com/docs/grid-archive/
published: true
dsq_thread_id:
  - "3848432144"
mashsb_timestamp:
  - 'a:1:{i:0;s:10:"1440715007";}'
mashsb_shares:
  - 'a:1:{i:0;s:1:"1";}'
mashsb_jsonshares:
  - 'a:1:{i:0;s:42:"{"total":1,"twitter":1,"facebook_total":0}";}'
---
Using JointsWP, you can easily display your posts in a grid format. The Grid Archive uses <a href="http://foundation.zurb.com/sites/docs/equalizer.html">Foundation's Equalizer</a> to ensure all posts are the same height, which keeps the grid intact.

In <code>index.php</code> or <code>archive.php</code> find:

[php]&lt;?php get_template_part( 'parts/loop', 'archive' ); ?&gt;[/php]

Change to:

[php]&lt;?php get_template_part( 'parts/loop', 'archive-grid' ); ?&gt;[/php]

<h3>Grid Archive Options</h3>
It is very easy to adjust the number of columns in the grid. Simply adjust the <code>$grid_columns</code> variable in <code>parts/loop-archive-grid.php</code> to the amount of columns you want to display. Then adjust the grid to your desired settings on line #13.

<p><a class="button" href="http://jointswp.com/demo/category/grid/" target="_blank">Grid Archive Demo</a></p>