---
ID: 312
post_title: >
  Using Foundation 6 Media Queries with
  Sass
author: Jeremy Englert
post_date: 2015-12-01 07:49:15
post_excerpt: ""
layout: post
permalink: >
  http://jointswp.com/using-foundation-6-media-queries-with-sass/
published: true
mashsb_timestamp:
  - "1478197646"
mashsb_shares:
  - "0"
mashsb_jsonshares:
  - '{"total":0,"facebook_total":0,"twitter":0}'
dsq_thread_id:
  - "4365175405"
---
In Foundation 6, the way we use media queries in our Sass files has changed just a bit compared to <a href="http://jointswp.com/using-foundation-media-queries-with-sass/" target="_blank">how things were done in Foundation 5</a>. We now have the ability to use the <a href="http://foundation.zurb.com/sites/docs/media-queries.html" target="_blank">breakpoint() mixin</a>, which makes using media queries with Sass even easier.

<!--more-->

For example, this Scss file:

[css]

.widget {
  padding: 0 5px;
  h1 {
    color: red;
    @include breakpoint(medium) {
      color: green;
    }
    @include breakpoint(large) {
      color: blue;
    }
  }
}

[/css]

compiles into CSS as:

[css]
.widget {
  padding: 0 5px;
}

.widget h1 {
  color: red;
}

@media only screen and (min-width: 40em) {
 .widget h1 {
   color: green;
 }
}

@media only screen and (min-width: 64em) {
 .widget h1 {
   color: blue;
 }
}
[/css]