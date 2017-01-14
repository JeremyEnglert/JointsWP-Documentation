---
ID: 205
post_title: WordPress Related Posts Without a Plugin
author: Jeremy Englert
post_date: 2015-02-10 08:09:21
post_excerpt: ""
layout: post
permalink: >
  http://jointswp.com/wordpress-related-posts-without-plugin/
published: true
dsq_thread_id:
  - "3502081088"
mashsb_timestamp:
  - "1478192911"
mashsb_shares:
  - "4"
mashsb_jsonshares:
  - '{"total":4,"twitter":4,"facebook_total":0}'
---
Finding a good "Related Posts" plugin can be hard. Many come with predefined styles or a rigid structure that makes them hard to integrate into your theme. Even worse, most of these plugins are extremely database intensive and some hosts, such as WP Engine, <a href="http://bit.ly/WPE-Banned-Plugins" target="_blank">won't even allow most "Related Post" plugins on their servers </a>(for good reason).

<!--more-->

The following code will display related posts by finding posts with the same tags as the current post. Simply add the code to your functions.php file and call it in your template using <code>joints_related_posts();</code>. <em>Note: If you're using <a title="Home" href="http://jointswp.com/" target="_blank">JointsWP</a>, this function is already built in. </em>

[php]
&lt;?php
// Related Posts Function, matches posts by tags - call using joints_related_posts(); )
function joints_related_posts() {
	global $post;
	$tags = wp_get_post_tags( $post-&gt;ID );
	if($tags) {
		foreach( $tags as $tag ) {
			$tag_arr .= $tag-&gt;slug . ',';
		}
		$args = array(
			'tag' =&gt; $tag_arr,
			'numberposts' =&gt; 3, /* You can change this to show more */
			'post__not_in' =&gt; array($post-&gt;ID)
		);
		$related_posts = get_posts( $args );
		if($related_posts) {
		echo '&lt;h4&gt;Related Posts&lt;/h4&gt;';
		echo '&lt;ul id=&quot;joints-related-posts&quot;&gt;';
			foreach ( $related_posts as $post ) : setup_postdata( $post ); ?&gt;
				&lt;li class=&quot;related_post&quot;&gt;
					&lt;a class=&quot;entry-unrelated&quot; href=&quot;&lt;?php the_permalink() ?&gt;&quot; title=&quot;&lt;?php the_title_attribute(); ?&gt;&quot;&gt;&lt;?php the_title(); ?&gt;&lt;/a&gt;
					&lt;?php get_template_part( 'partials/content', 'byline' ); ?&gt;
				&lt;/li&gt;
			&lt;?php endforeach; }
			}
	wp_reset_postdata();
	echo '&lt;/ul&gt;';
}
?&gt;
[/php]

This code is very, very similar to the code found in <a href="https://github.com/eddiemachado/bones" target="_blank">Bones</a> - however, it has been modified so that if no related posts are found, the "Related Posts" section will not display.