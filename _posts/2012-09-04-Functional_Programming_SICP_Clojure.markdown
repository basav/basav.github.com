--- 
layout: post
title: Functional Programming - SICP - Clojure
category: coding learning 
tags: sicp clojure github 
year: 2012
month: 09
day: 04
published: true 
summary:
---
<div class="row">
      <div class="span3 columns well">
        <h3>About this topic</h3>
        <p>Blog summary</p>
        <br>
        <h3>Topic buzz</h3>
        <p>What others are thinking. Add to the conversation and
          generate some chatter.</p>
        <p><a href="https://twitter.com/share"
            class="twitter-share-button" data-via="basav">Tweet</a></p>
        <p><g:plusone size="medium"></g:plusone></p>
        <br>
        <h3>Read later</h3>
        <p>Save this article for a later read or point of reference.        <a
href="http://www.instapaper.com/hello2?url=http://basav.github.com{{ page.url }}&amp;title={{ page.title }}"
title="Save {{ page.title }} to Instapaper" target="_blank">+Instapaper</a>
        </p>
        <br>
      </div>
      <div class="span8 columns">
        <p> <a href="http://en.wikipedia.org/wiki/Functional_programming">Functional

            Programming</a> is hard. Especially for experienced folks
          who have been working with <a href="http://en.wikipedia.org/wiki/Object-oriented_design">
            Object oriented </a> concepts all these years. More-over
          universities are including Java as the mainstream language in
          the course curriculum and moving away from C or Lisp
          completely. Check this <a href="http://www.joelonsoftware.com/articles/ThePerilsofJavaSchools.html">fantastic article</a> by Joel Spolsky - who highlights the <b>adverse effect</b> of such a shift.&nbsp; He writes how important it
          is to understand the concept of pointers and functional
          programming constructs. Agreed that pointers are no more used
          in any production code these days and neither functional
          constructs are not widely adopted - but these are required to
          understand the very <i><b>fundamentals</b></i> of computer
          programming and how to build complex software. He writes "<i>You
            can't understand a line of code in Linux, or, indeed, any
            operating system, without really understanding pointers.
            Without understanding functional programming, you can't
            invent <a href="http://en.wikipedia.org/wiki/Map_reduce">MapReduce</a>,
            the algorithm that makes Google so massively scalable. The
            terms Map and Reduce come from <a href="http://en.wikipedia.org/wiki/Lisp">Lisp</a> and
            functional programming."
          </i></p>
          <br>
        <hr>
        <h2>SICP<
        </h2>
        <hr> </div>
    </div>
    <div class="row">
      <div class="span3 columns">&nbsp;<br>
        There is no better way to learn the concepts of functional and
        recursive programming - other than from excellent <a href="http://sicp.csail.mit.edu/Fall-2007/">course
      </a> created
        by the best university in the world - <a href="http://en.wikipedia.org/wiki/MIT">MIT</a>.
        <a href="http://en.wikipedia.org/wiki/Structure_and_Interpretation_of_Computer_Programs">SICP

        </a>is a textbook published by <a href="http://en.wikipedia.org/wiki/MIT_Press">MIT Press</a>
        and it was formerly used to teach introductory programming class
        for students at MIT and other various universities.&nbsp; MIT
        has set a very high bar and the course material is hard.
        Fortunately there are about 20 actual video lectures shot at MIT
        are available <a href="http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-001-structure-and-interpretation-of-computer-programs-spring-2005/video-lectures/">online</a>
        which help in digesting some of the tough concepts. Plus there
        are <a href="https://www.google.com/#hl=en&amp;sclient=psy-ab&amp;q=sicp+study+group">study-groups</a>,
        <a href="http://stackoverflow.com/questions/tagged/sicp">stackoverflow</a>
        to help crack some tough nuts.
        
        <img alt="SICP book cover image" src="http://mitpress.mit.edu/sicp/full-text/book/cover.jpg"><br>
        The <i><b>eval-apply </b></i>loop on the above front cover
        show the relationship between data and programs and the <i><b>lambda</b></i>
        emphasizing that functions are indeed type of data. Functions
        are treated as first class citizens (or objects), which is the
        heart of this paradigm and this is not present in languages as
        Java or C. Thinking functions as first-class objects helps in
        understands the important concept of <b>abstraction </b>and
        abstraction is very important to build large scale software
        systems<br>
      </div>
      <div class="span9 column">
        <p class="pull-right">{% if page.previous.url %} {% endif %} {%
          if page.next.url %} {% endif %} </p>
      </div>
    </div>
    <div class="row">
      <div class="span3 columns">&nbsp;</div>
      <div class="span9 columns">
        <h2>Comments Section</h2>
        <p>Feel free to comment on the post but keep it clean and on
          topic.</p>
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
			</script> <noscript>Please enable JavaScript to view the <a href="http://disqus.com/?ref_noscript">comments powered by Disqus.</a></noscript>
        <a href="http://disqus.com" class="dsq-brlink">blog comments
          powered by <span class="logo-disqus">Disqus</span></a> </div>
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

