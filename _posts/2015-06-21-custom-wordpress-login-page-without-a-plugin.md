---
ID: 277
post_title: >
  Custom WordPress Login Page Without a
  Plugin
author: Jeremy Englert
post_date: 2015-06-21 22:38:10
post_excerpt: ""
layout: post
permalink: >
  http://jointswp.com/custom-wordpress-login-page-without-a-plugin/
published: true
mashsb_timestamp:
  - "1478152108"
mashsb_shares:
  - "2"
mashsb_jsonshares:
  - '{"total":2,"twitter":1,"facebook_total":1}'
dsq_thread_id:
  - "3867633469"
---
It's really easy to add custom styles to your WordPress login page without needing to install a plugin.

<!--more-->

Simply add the following to your functions.php file:

[php]
&lt;?php
// Calling your own login css so you can style it
function joints_login_css() {
	wp_enqueue_style( 'joints_login_css', get_template_directory_uri() . '/login.css', false );
}

// Changing the logo link from wordpress.org to your site
function joints_login_url() {  return home_url(); }

// Changing the alt text on the logo to show your site name
function joints_login_title() { return get_option('blogname'); }

// Calling it only on the login page
add_action( 'login_enqueue_scripts', 'joints_login_css', 10 );
add_filter('login_headerurl', 'joints_login_url');
add_filter('login_headertitle', 'joints_login_title');
?&gt;
[/php]

You'll also need to create a new stylesheet for your login styles. Here is some basic styling you can use to change the logo of the login page:

[css]
.login h1 a {
  background: url(../images/login-logo.png) no-repeat top center;
  /* Make sure to update these with the dimensions of your logo */
  width: 326px;
  height: 67px;
  text-indent: -9999px;
  overflow: hidden;
  padding-bottom: 15px;
  display: block;
}

[/css]

This code comes included with <a href="http://jointswp.com/" target="_blank">JointsWP</a> and is very similar to the code found in <a href="http://themble.com/bones/" target="_blank">Bones</a>.