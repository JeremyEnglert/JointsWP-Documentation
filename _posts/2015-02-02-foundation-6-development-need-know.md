---
ID: 130
post_title: 'Foundation 6 is in Development &#8211; What You Need to Know'
author: Jeremy Englert
post_date: 2015-02-02 02:20:57
post_excerpt: ""
layout: post
permalink: >
  http://jointswp.com/foundation-6-development-need-know/
published: true
dsq_thread_id:
  - "3474098735"
mashsb_timestamp:
  - "1484336463"
mashsb_shares:
  - "142"
mashsb_jsonshares:
  - '{"total":142,"facebook_total":27,"twitter":115}'
---
<strong>UPDATED 6/22/15 - </strong><em>Added information about optional build template that will include UnCSS</em>

<em><strong>UPDATED 2/9/15 - </strong>Added information about the optional Flexbox Grid and Motion UI integration</em>

The team at ZURB is at it again!

Fresh of the heels of their successful <a href="http://zurb.com/article/1362/foundation-for-apps-is-here" target="_blank">Foundation for Apps launch</a>, the Foundation team has announced they have started the development of Foundation (for Sites) 6. While nothing is official yet, there are some very interesting discussions and comments on GitHub about the newest release of the popular framework.

<!--more-->
<h3>When will Foundation 6 be released?</h3>
It is much too early to make any type of assumption about when Foundation 6 will be released, however, it's safe to say it will be in development for at least the next few months.
<h3>What will be new?</h3>
As noted above, nothing has been made official, but the ZURB team has given some indication of their plans for the new release.
<h4>The Grid - Awesome Gets Awesome-er</h4>
The grid system has always been one of the most useful and powerful features packaged into Foundation. However, in the last couple of years, new grid system frameworks (Susy, Zen, Singularity) have been gaining popularity. Look for the next version of the Foundation grid to include multiple grid column counts and simpler Sass markup - allowing it to compete with these more advanced grid systems.

Flexbox was used in Foundation for Apps and will most likely be included in Foundation 6 as an optional grid system.
<h4>Slimming Down - Some Components May be Deprecated</h4>
I was excited to hear that there are plans to cut back on the amount of components and plugins found in the core of the framework. Here are some of the components likely to be deprecated:
<ul class="task-list">
	<li>Block grid - not necessarily deprecated, but will be merged into the primary grid</li>
	<li>Top bar - will be replaced by a new, less opinionated version</li>
	<li>Orbit - Orbit was actually deprecated in an earlier version of Foundation, however, it may return as a simple image slider with basic features</li>
	<li>Clearing</li>
	<li>Pricing tables</li>
</ul>
Some components may be taken out of the core and become their own <a href="http://patterntap.com/code" target="_blank">"plugins" which can easily be added to Foundation projects</a>. There has also been discussions of adding new components such as a mega menu and a sticky navigation.
<h4>Components Re-Written for Accessibility</h4>
Foundation 5 took large leaps in terms of accessibility and the goal for Foundation 6 is for all components to be 100% accessible.
<h4>Foundation JavaScript Re-Written from Scratch</h4>
The JavaScript packaged with Foundation 5 is nearly 18 months old, which has led the Foundation team to lean towards re-writing it from scratch. They also plan on integrating a 'Common API' for JavaScript components to take advantage of. This should make working with JavaScript components much easier as they will all share a common set of commands.
<h4>Motion UI Integration</h4>
The <a href="http://foundation.zurb.com/apps/docs/#!/motion-ui">Motion UI</a> uses Sass mixins and CSS animations to create easy-to-use animation effects. The Motion UI was originally part of the Foundation for Apps framework, but all indications point to it being included in Foundation 6.
<h4><span style="top:-5px;" class="label">Update</span> Optional Build Templates and UnCSS</h4> 
The Foundation team recently <a href="http://foundation.zurb.com/forum/posts/25541-" target="_blank">posted on the forums</a> that Foundation 6 "will have an optional build template, like Assemble with UnCSS included into the build."

While <a href="https://github.com/giakki/uncss" target="_blank">UnCSS</a> in itself is awesome, I think the more exciting news is <em><strong>optional build templates</strong></em>. Similar to how Foundation 6 will offer additional features as "plugins", it sounds like they will also offer additional build templates that can be used for different purposes. Imagine having a Grunt file pre-setup for WordPress development, or a Grunt file specific to rapid prototyping - these build templates could be huge time savers.
<h3>How can I get involved?</h3>
The Foundation Team is looking to the community for ideas and feedback on Foundation 6. They recently gathered all of the feedback from GitHub and moved it to a public Trello board so the community can vote on upcoming features - <a href="https://trello.com/b/QBPKlQqf" target="_blank">check it out here</a>. If you have any ideas on how Foundation can be improved, now is your chance to get involved.

Which Foundation 6 feature are you most excited for? Comment below!