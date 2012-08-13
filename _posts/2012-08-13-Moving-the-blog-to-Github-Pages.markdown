---
layout: post
title: Moving my blog to Github Pages
category: Coding
tags: jekyll bootstrap github disqus
year: 2012
month: 8
day: 13
published: true
summary: It's about time..moving my blog to Github Pages
---

<div class="row">
	<div class="span3 columns well">
	  <h3>About this topic</h3>
	  <p>Moving my blog to Githug Pages. This post outlines some of my experiences of doing so</p>	  
	  <br/>
	  <h3>Topic buzz</h3>
	  <p>What others are thinking. Add to the conversation and generate some chatter.</p>
	  <p><a href="https://twitter.com/share" class="twitter-share-button" data-via="basav">Tweet</a></p>
	  <p><g:plusone size="medium"></g:plusone></p>
	  <br/>
	  <h3>Read later</h3>
	  <p>Save this article for a later read or point of reference. <a href="http://www.instapaper.com/hello2?url=http://basav.github.com{{ page.url }}&title={{ page.title }}" title="Save {{ page.title }} to Instapaper" target="_blank">+Instapaper</a> </p>
	  <br/>  
	</div>	
	<div class="span8 columns">
	 	<p> 
		 It was about time that I stopped procrastinating and start writing my blog regularly. So I switched to a lean blogging framework <a href="http://jekyllbootstrap.com/index.html#start-now"> Jekyll </a> powered by <a href="http://pages.github.com"> Github Pages </a>. It's extremely developer friendly. Writing and sharing code snippets with Gist should be easy.
		</p>
	  <hr>
		  <h2>Why?</h2>
		<ul> 
			<li> Manage everything with git </li>
			<li> Can blog on when there is no Internet connection (at airports, train rides etc) </li>
			<li> Power of Git - everything tracked, you have your complete blog on your laptop </li>
			<li> Lightweight etc etc</li>
		</ul>	
	  <hr>
		  <h2>How?</h2>	
		<p>
			Thanks to this awesome post from <a href="http://erjjones.github.com/blog/How-I-built-my-blog-in-one-day/"> Eric  </a>. Just follow the steps outlined and it's the quickest way to have something up and running. With most of the heavy-lifting done, should not take more than few hours to move to Pages.
		</p>
		<p>
		<a href="https://gist.github.com/kennym"> Kennym's </a> nice script helped to moved some of my posts from Blogger to Jekyll. The gist can be found 	<a href="https://gist.github.com/1115810"> here </a>.
			</p>
			<hr>
			  <h2>Conclusion</h2>	
			The web is having a uniform look and feel because of Twitter Bootstrap theme and design practices. Some like it and some don't like it. I like it - its clean, easy and quick. I was looking for <a href="https://github.com/mojombo/jekyll/wiki/sites"> Github Pages Sites </a> with Twitter Bootstrap integration. I found this on Eric's Github. I had even experimented something on my own integrating Bootstrap but had got stuck and left it halfway. So I just reused something already available :).
			Some work still needs to be done - like pagination of posts, some social networks integration etc. But that is for any day..
		
	</div>
</div> 

<div class="row">
	<div class="span3 columns">&nbsp;</div>
	<div class="span9 column">
			<p class="pull-right">{% if page.previous.url %} <a href="{{page.previous.url}}" title="Previous Post: {{page.previous.title}}"><i class="icon-chevron-left"></i></a> 	{% endif %}   {% if page.next.url %} 	<a href="{{page.next.url}}" title="Next Post: {{page.next.title}}"><i class="icon-chevron-right"></i></a> 	{% endif %} </p>  
	</div>
</div>

<div class="row">
	<div class="span3 columns">&nbsp;</div>
    <div class="span9 columns">    
		<h2>Comments Section</h2>
	    <p>Feel free to comment on the post but keep it clean and on topic.</p>	
		<div id="disqus_thread"></div>
		<!-- Put this just before the closing body tag of your web page -->
		<script type="text/javascript">
				/* * * CONFIGURATION VARIABLES: EDIT BEFORE PASTING INTO YOUR WEBPAGE * * */
				var disqus_shortname = 'basav'; // required: replace example with your forum shortname
		        var disqus_identifier = '{{ page.url }}';
				var disqus_url = 'http://basav.github.com{{ page.url }}';
				console.log(disqus_url);
				/* * * DON'T EDIT BELOW THIS LINE * * */
				(function () {
					var s = document.createElement('script'); s.async = true;
					s.type = 'text/javascript';
					s.src = 'http://' + disqus_shortname + '.disqus.com/count.js';
					(document.getElementsByTagName('HEAD')[0] || document.getElementsByTagName('BODY')[0]).appendChild(s);
				}());
			</script>
		<noscript>Please enable JavaScript to view the <a href="http://disqus.com/?ref_noscript">comments powered by Disqus.</a></noscript>
		<a href="http://disqus.com" class="dsq-brlink">blog comments powered by <span class="logo-disqus">Disqus</span></a>
	</div>
</div>

<!-- Twitter -->
<script>!function(d,s,id){var js,fjs=d.getElementsByTagName(s)[0];if(!d.getElementById(id)){js=d.createElement(s);js.id=id;js.src="//platform.twitter.com/widgets.js";fjs.parentNode.insertBefore(js,fjs);}}(document,"script","twitter-wjs");</script>

<!-- Google + -->
<script type="text/javascript">
  (function() {
    var po = document.createElement('script'); po.type = 'text/javascript'; po.async = true;
    po.src = 'https://apis.google.com/js/plusone.js';
    var s = document.getElementsByTagName('script')[0]; s.parentNode.insertBefore(po, s);
  })();
</script>