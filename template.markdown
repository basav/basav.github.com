---
layout: post
title: 
category: 
tags: 
year: 
month: 
day: 
published: true
summary: 
---

<div class="row">
	<div class="span3 columns well">
	  <h3>About this topic</h3>
	  <p>Blog summary</p>	  
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
			Blog Description
		</p>
	  <hr>
		  <h2>Header</h2>
	  <hr>
		
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
				/* * * DON'T EDIT BELOW THIS LINE * * */
				(function() {
				var dsq = document.createElement('script'); dsq.type = 'text/javascript'; dsq.async = true;
				dsq.src = 'http://' + disqus_shortname + '.disqus.com/embed.js';
				(document.getElementsByTagName('head')[0] || document.getElementsByTagName('body')[0]).appendChild(dsq);
			})();
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