---
ID: 365
post_title: Admin Functions
author: Jeremy Englert
post_date: 2016-01-04 08:19:34
post_excerpt: ""
layout: page
permalink: >
  http://jointswp.com/docs/admin-functions/
published: true
dsq_thread_id:
  - 'a:1:{i:0;s:10:"4459662527";}'
---
Simple functions that allow for the customization of the WordPress dashboard.

These functions are turned off by default. To activate them, locate the following line in functions.php and uncomment it:

[php]require_once(get_template_directory().'/assets/functions/admin.php');[/php]

These functions are located in <code>assets/functions/admin.php</code>.

<h3>Remove Dashboard Widgets</h3>
<code>disable_default_dashboard_widgets()</code> function removes annoying dashboard widgets that are installed by WordPress core and popular plugins.
<h3>Custom RSS Dashboard Widget</h3>
<code>joints_rss_dashboard_widget()</code> function allows for a custom RSS feed to be embdeded into the WordPress dashboard. Simply replace the URL with the URL of your feed.
<h3>Custom RSS Dashboard Widget</h3>
<code>joints_custom_admin_footer()</code> functions allows for the customization of the "Thank you for creating with WordPress" text found at the bottom of the WordPress dashboard.