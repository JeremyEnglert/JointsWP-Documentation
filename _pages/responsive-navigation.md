---
ID: 354
post_title: Responsive Navigation
author: Jeremy Englert
post_date: 2016-01-04 07:34:47
post_excerpt: ""
layout: page
permalink: >
  http://jointswp.com/docs/responsive-navigation/
published: true
dsq_thread_id:
  - 'a:1:{i:0;s:10:"4459576949";}'
---
The responsive topbar uses <a href="http://foundation.zurb.com/sites/docs/responsive-navigation.html" target="_blank">Foundation 6 Responsive Navigation Patterns</a> to make it easy to switch between accordion, dropdown and drilldown menus at different breakpoints.

To use this menu type, change the template part in <code>header.php</code> to:

[php]&lt;?php get_template_part( 'parts/nav', 'topbar' ); ?&gt;[/php]

<h3>Responsive Menu Options</h3>
In the <code>functions/menu.php</code> file, locate the <code>joints_top_nav()</code> function. The two important lines of code are:

[php]
'menu_class' =&gt; 'vertical medium-horizontal menu',
'items_wrap' =&gt; '&lt;ul id=&quot;%1$s&quot; class=&quot;%2$s&quot; data-responsive-menu=&quot;accordion medium-dropdown&quot;&gt;%3$s&lt;/ul&gt;',
[/php]

Simply update the <code>menu_class</code> and <code>items_wrap</code> to match the navigation pattern you want. You also may need to adjust the class in <code>assets/functions/menu.php</code> depending on the type of menu you are creating.
