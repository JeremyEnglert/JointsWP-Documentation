---
ID: 237
post_title: >
  Using Foundation 5 Media Queries with
  Sass
author: Jeremy Englert
post_date: 2015-06-14 21:39:40
post_excerpt: ""
layout: post
permalink: >
  http://jointswp.com/using-foundation-media-queries-with-sass/
published: true
mashsb_timestamp:
  - "1478192243"
mashsb_shares:
  - "4"
mashsb_jsonshares:
  - '{"total":4,"twitter":4,"facebook_total":0}'
dsq_thread_id:
  - "3848570541"
---
<strong>Updated Post: </strong><a href="http://jointswp.com/using-foundation-6-media-queries-with-sass/">Using Foundation 6 Media Queries with Sass</a>

The Foundation Grid comes with <a href="http://foundation.zurb.com/docs/media-queries.html" target="_blank">predefined media queries</a> that can be nested into your Sass styles to create specific styles for different screen sizes.

<!--more-->

For example, this Scss file:

[css]

.widget {
  padding: 0 5px;
  h1 {
    color: red;
    @media #{$medium-up} {
      color: green;
    }
    @media #{$large-up} {
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

@media only screen and (min-width: 40.0625em) {
 .widget h1 {
   color: green;
 }
}

@media only screen and (min-width: 64.063em) {
 .widget h1 {
   color: blue;
 }
}
[/css]