---
ID: 299
post_title: Foundation 6 Meets WordPress
author: Jeremy Englert
post_date: 2015-11-19 21:17:34
post_excerpt: ""
layout: post
permalink: >
  http://jointswp.com/foundation-6-meets-wordpress/
published: true
mashsb_timestamp:
  - "1478186271"
mashsb_shares:
  - "53"
mashsb_jsonshares:
  - '{"total":53,"facebook_total":53,"twitter":0}'
dsq_thread_id:
  - "4334097530"
---
<a href="http://zurb.com/article/1416/foundation-6-is-here">Foundation (for Sites) 6</a> is officially here, which means <a href="http://jointswp.com/" target="_blank">JointsWP 4 is also here</a>! As in previous versions of JointsWP, the theme is essentially "blank" but includes all of the awesome features of Foundation 6. Let's take a look at what's new in Foundation 6 and how it effects JointsWP 4.

<!--more-->
<h2>What's new in Foundation 6?</h2>
<h3>No More Bloat</h3>
CSS frameworks have always had an unjust reputation of being "bloated" - Foundation 6 is changing that. Most of the JavaScript components have been rewritten and the restructuring of Sass files to be "<a href="http://zurb.com/article/1407/foundation-6-leaner-meaner-and-cleaner-sa" target="_blank">leaner, meaner and cleaner</a>" means you can expect a 40-50% smaller output when using Foundation 6 compared to Foundation 5. The Sass restructuring also makes it extremely easy to select which Sass components you want to include - so you won't have a ton of extra styles you never plan on utilizing.

If you consider Foundation 6 "bloated", you're doing it wrong.
<h3>Menus Receive a Super Sexy Makeover</h3>
Modifying the "top bar" in Foundation 5 was far from fun - if you wanted to do anything besides change a few colors, you were in for a lot of work.

In Foundation 6, the "top bar" has now been split up into 3 separate menu types - a dropdown menu, an accordion menu and a drilldown menu. Using the responsive navigation patterns will allow you to implement different menus on specific screen sizes.

For example, a dropdown menu may look great on a desktop device but be better suited as an accordion menu on smaller devices - with Foundation 6 and JointsWP 4, you only need to adjust a few classes to make this happen.
<h3>Accessibility &amp; What-Input</h3>
The ZURB team put a lot of work into making sure Foundation 6 is as accessible as possible. One really cool feature is the addition of <a href="https://github.com/ten1seven/what-input" target="_blank">What-Input</a>, which allows developers to create separate styles based on whether the user is using a keyboard or a mouse. This means developers can keep important accessibility elements such as outlines visible to users using a keyboard, but set the outlines to be hidden if the site is being navigated with a mouse.
<h3>That's Not All, Folks</h3>
This just scratches the surface of the changes that came to Foundation 6. Other useful features include:
<ul>
	<li><strong>Flex Grid</strong> - developers can now use the flex grid using the same markup they used in the traditional/float grid, but with a lot more flexibility (pun completed intended)</li>
	<li><strong><a href="http://zurb.com/article/1409/introducing-the-new-motion-ui" target="_blank">Motion-UI</a> </strong>- this will be included by default in Foundation 6 and allows developers to quickly create their own motion effects or use existing effects created by the Foundation team.</li>
	<li><strong>Off-Canvas Improvements</strong> - no longer strictly used for menus, the off-canvas component in Foundation 6 will act much more like a container that can hold all types of content.</li>
	<li>So, so, so much more.</li>
</ul>
<h2>What's new in JointsWP 4?</h2>
The primary purpose of this was release was to integrate Foundation 6 into JointsWP, however, other small changes were made as well.
<ul>
	<li><strong>Improved File Structure - </strong>my weird obsession with file structure continues. Vendor files, such as Foundation and jQuery now live inside a /vendor/ directory. This makes it extremely easy to update these assets, even if you aren't using Bower.</li>
	<li><strong>Improved Loop Structure -</strong> the new loop structure makes it easier to include template parts and also allows for custom error messages to be created much more easily.</li>
	<li><b>Gulp &amp; Bower Working Together -</b> Run gulp bower to automatically update all vendor files. Bower will create a new bower_components directory and then automatically copy the updated files to your /vendor/ directory. Awesome stuff.</li>
	<li><strong>Better Translation Support - </strong>All  text/strings should now be fully translation ready.</li>
</ul>
Had a chance to check out JointsWP 4? Excited for Foundation 6?  Let's chat below.