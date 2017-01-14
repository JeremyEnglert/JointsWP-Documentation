---
ID: 194
post_title: >
  CSS Frameworks Are a Great Tool for
  WordPress Developers
author: Jeremy Englert
post_date: 2015-02-20 09:15:05
post_excerpt: ""
layout: post
permalink: >
  http://jointswp.com/css-frameworks-for-wordpress-developers/
published: true
dsq_thread_id:
  - "3528462298"
mashsb_timestamp:
  - "1478192962"
mashsb_shares:
  - "72"
mashsb_jsonshares:
  - '{"total":72,"twitter":63,"facebook_total":9}'
---
<em><strong>UPDATED 2/25/15 – </strong>Added information about use of Foundation mixins for styling WordPress components
</em>

In August, ThemeShaper posted, <a href="http://themeshaper.com/2014/08/19/why-bootstrap-is-a-bad-fit-for-wordpress-themes/" target="_blank">"Why Bootstrap is a Bad Fit For WordPress Themes"</a>. While I initially thought the author had issues with Bootstrap specifically, it appears the article was actually targeted towards all CSS frameworks, including Foundation.

Some of the arguments being made, such as having to overwrite default styling (which is more of an issue with Bootstrap than Foundation) are completely valid. However, there were also some misconceptions being thrown around that I would like to clear up.

<!--more-->
<h3>Misconception #1 - Frameworks are bloated</h3>
This is often a complaint about CSS frameworks and basically every other piece of code...ever, including WordPress. We've fallen into a mindset that if a framework or library has too many features or features we don't use often, that it automatically means that the code is "bloated". However, the entire point of using a framework is to speed up development and have components that are ready to use - so "bloat" (if you insist on calling it that) is to be expected.

Fortunately, most frameworks (Foundation especially), make it very easy to remove components you are not using - essentially making the complaints about "bloat" a moot point. However, since most developers seem to skip the step of removing unused components, the <a href="http://zurb.com/article/1373/hit-the-weights-and-take-the-bloat-out-of" target="_blank">Foundation 6 core will be slimmed down</a> and only come with essential components while additional components can easily be added.
<h3>Misconception #2 - Frameworks don't do things the 'WordPress Way'</h3>
I think its time we look at this from a different perspective. If developers <strong><em>have</em></strong> to do things "the WordPress way" in order for them to work, maybe "the WordPress way" is really the problem.

If WordPress wants to continue to grow and reach their goal of 50% market share, they're going to need to make the platform more friendly to modern developer workflows - especially as it continues to grow as a platform for web applications.

As pointed out by Rafi in the comments, Foundation also includes every component as a mixin. Meaning you can easily style core WordPress elements and plugins without ever needing to use the Foundation class names or modify existing class names.

Additionally, If you're starting with a blank developers theme - <em>ahem, <a href="http://jointswp.com/">JointsWP</a></em> - the integration with WordPress is already in place.
<h2>Are They a Good Tool for WordPress Developers? Yes!</h2>
<h3>Less Bloat</h3>
Yes, you read that right. Using a CSS Framework may actually cut back on the amount of "bloat" in your WordPress theme. Foundation and Bootstrap both come with components such as drop down modals, slideshows, sticky navigation and more. These are all common elements among websites that would otherwise require downloading an additional plugin or writing additional code to get the same functionality.

Not only do you use less plugins, but the components included in the framework are already built to work with the rest of your website.
<h3>Common Code Among Teams</h3>
Have you ever been handed a project smack-dab in the middle of development? If so, you already know that much of your time will be spent figuring out exactly what the previous developer was doing and the structure he/she was trying to follow.

If your team is using a CSS framework, this is no longer an issue. Your entire team will be using one set of common code and projects can easily be passed between team members without any hiccups.
<h3>Faster Development</h3>
Sure, you will have to spend some time overwriting a few default styles, but is that really more time-consuming than writing components such as buttons or drop-downs from scratch? Doubtful. Plus, framework components are being used by thousands of developers everyday who are actively testing for bugs and improving the code.

What do you think? Are Foundation and Bootstrap good tools for WordPress developers? Comment below.