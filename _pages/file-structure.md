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
## Sass Version
### Custom Styles
* `style.css` - this file is never actually loaded, however, this is where you set your theme name and is required by WordPress
* `assets/styles/scss/style.scss` - import all of your styles here. If you create an additional SCSS file, be sure to import it here.
* `assets/styles/scss/_main.scss` - place all of your custom styles here.
* `assets/styles/scss/_settings.scss` - adjust Foundation style settings here.
* `assets/styles/scss/login.scss` - place custom login styles here. This will generate it's own stylesheet.

### Custom Scripts
* `assets/scripts/js/` - place your custom scripts here. Each .JS file will be compiled and concatenated when the build process is ran.

### Images
* `assets/images/` - place your theme images here. Each image will be optimized when the build process is ran.

## CSS Version
Coming soon. 
