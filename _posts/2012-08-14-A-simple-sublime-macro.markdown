---
layout: post
title: Delete Line Sublime Macro
category: tools
tags: sublime
year: 2012
month: 8
day: 14
published: true
summary: Command + D to delete line in Sublime 2
---

<div class="row">
	<div class="span3 columns well">
	  <h3>About this topic</h3>
	  <p>Command + D to delete line in Sublime 2</p>	  
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
			Sublime 2 Text editor does not have by default have a key binding to delete the current line. The alternative way is to select the entire line i.e. by <b>Command + L </b>and then pressing backspace. I'm so used to <b>Command + D</b> command to delete the current line.
		</p>

	  <hr>
		<p>
			The easiest way to get this done is by recording a macro with these two commands and then binding <b>Command + D</b> to this user defined macro.
			You can use the <b>Tools</b> menu to record a macro with the above two commands. The macros are by default stored in <b>Packages/User/</b> directory. 
			The other option is to just create a new file with the below text. 
			<p>

			<script src="https://gist.github.com/3388743.js"></script>

			</p>
			Save the file as <b>Delete-Line.sublime-macro</b> in 
			<b>/yourhomedirectory/Library/Application Support/Sublime Text 2/Packages/User/</b> directory. 
		</p>
		<p>
			Next step would be to bind <b>Command + D</b> to this macro. This can be accomplished by adding a User Key Binding. 
			Navigate to <b>Sublime Text 2 | Preferences | Key Bindings - User </b> menu and add (or append if you already have any custom key bindings) the below line
			<p> <script src="https://gist.github.com/3388756.js"></script>
			</p>
		</p>
		 <hr>
		 <p>
		 	This should take care of it.
		 </p>
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