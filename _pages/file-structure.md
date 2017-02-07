---
ID: 339
post_title: File Structure
author: Jeremy Englert
post_date: 2015-12-11 06:04:21
post_excerpt: ""
layout: page
permalink: http://jointswp.com/docs/file-structure/
published: true
dsq_thread_id:
  - 'a:1:{i:0;s:10:"4420813762";}'
---
<h2>Sass Version</h2>
<h3>Styles</h3>
<code>styles.css</code> - A file required by WordPress, but not used.

<code>assets/scss/style.scss</code> - Import all of your Sass files here. This file also imports all Foundation styles from the <code>vendor</code> directory. You can remove whatever components you don't plan on using.

<code>assets/scss/_main.scss</code> - This is where you will put most of your custom styles

<code>assets/scss/_settings.scss</code> - Override Foundation styles and variables

<code>assets/css/*.css</code> - This is where all of the Sass files will compile. Don't edit these files directly as they will be overwritten anytime you compile your Sass.
<h3>Scripts</h3>
<code>assets/js/foundation.js</code> - Foundation JS files. If you're using Gulp, this compiles all Foundation JavaScript components from <code>vendor/foundation-sites/js</code>. You can select which components you want by making adjustments to the <code>gulpfile.js</code>. This file also comes in a minified form.

<code>assets/js/scripts.js</code> - This is where all of your custom JavaScript will go. If you're using Gulp, this compiles all Foundation JavaScript components from assets<code>/js/scripts</code>.. This file also comes in a minified form.

<code>assets/js/scripts/*.js</code> - If you're using Gulp, you can place all of your custom JS files here and they will be compiled into the <code>assets/js/scripts.js</code> file.
<h3>Vendor</h3>
<code>vendor/</code> - All vendor files are located here. It is not recommended to make changes to these files (except when updating).

<hr />

<h2>CSS Version</h2>
<code>styles.css</code> - A file required by WordPress, but not used.

<code>assets/css/style.css</code> - Place custom styles here.

<code>assets/js/scripts.js</code> - Place JavaScript here.

<code>vendor/</code> - Foundation and other vendor files are loaded from here. It is not recommended to make changes to these files (except when updating).