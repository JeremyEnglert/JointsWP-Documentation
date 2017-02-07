---
ID: 360
post_title: Off-Canvas Top Bar
author: Jeremy Englert
post_date: 2016-01-04 07:55:54
post_excerpt: ""
layout: page
permalink: >
  http://jointswp.com/docs/off-canvas-top-bar/
published: true
dsq_thread_id:
  - 'a:1:{i:0;s:10:"4459622965";}'
---
This is a combination of the <a href="http://jointswp.com/docs/off-canvas-menu/">Off-Canvas</a> and <a href="http://jointswp.com/docs/responsive-navigation/">Responsive Top Bar</a> menus. On small screens, an off-canvas menu will be used; on medium and larger screens, the responsive navigation patterns will be utilized. To use this menu type, change the template part in <code>header.php</code> to:

[php]&lt;?php get_template_part( 'parts/nav', 'offcanvas-topbar' ); ?&gt;[/php]

<h3>Off-Canvas Top Bar Settings</h3>
By default, an off-canvas menu will be triggered on small screens. This can be adjusted in the <code>parts/nav-offcanvas-topbar.php</code> file.

<a class="button" href="http://jointswp.com/demo/off-canvas-top-bar/">View Off-Canvas Top Bar Demo</a>