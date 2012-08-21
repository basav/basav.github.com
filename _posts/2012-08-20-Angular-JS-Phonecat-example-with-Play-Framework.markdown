--- 
layout: post
title: Angular Phonecat with Play Framework
category: coding
tags: angular play-framework github tech 
year: 2012
month: 8
day: 20
published: true
summary: Using Angular js Example App with Play Framework 2.0
---
<div class="row">

    <div class="span3 columns well">
        <h3>About this topic</h3>

        <p>Using Angular JS Framework inside Play Framework 2.0 Java</p>
         <p><a href="https://github.com/basav/momo/zipball/master" class="btn btn-info">Download source</a></p>
        <br>

        <h3>Topic buzz</h3>

        <p>
            What others are thinking. Add to the conversation and generate some chatter.
        </p>

        <p>
            <a href="https://twitter.com/share" class="twitter-share-button">Tweet</a>
        </p>

        <p>
            <g:plusone size=medium></g:plusone>
        </p>
        <br>

        <h3>Read later</h3>

        <p>
            Save this article for a later read or point of reference.
            <a
href="http://www.instapaper.com/hello2?url=http://basav.github.com{{ page.url }}&amp;title={{ page.title }}"
title="Save {{ page.title }} to Instapaper" target="_blank">+Instapaper</a>
        </p>
        <br></div>

    <div class="span8 columns">
        <p>
            After lot of debate and discussion - fellow geeks at my work have decided to
use <a href="http://angularjs.org/"> Angular JS </a> as the standard for the Javascript <a href="http://en.wikipedia.org/wiki/Model-view-controller">MVC</a> library. <a href="http://emberjs.com/">Ember.js</a> came
very close but Angular beat Ember.
        </p>

        <p>
            I'm quite familiar with <a href="http://www.playframework.org/">Play framework</a>. Both 1.2.x versions as well as Play
2.0 Java version. I'm learning the basics of Angular JS. Angular folks have put
up excellent <a href="http://docs.angularjs.org/tutorial">documentation</a> on their site with step-wise tutorials. I also like
the structure of the tutorials - step wise - focussing on TDD and
leveraging git diff at each step to show how the code evolves. A neat and powerful
concept to educate new frameworks and code-base.
        </p>

        <p>
            Angular JS Phonecat tutorial is a standalone app where the content is served
from the json files. I have integrated this example app with Play Framework 2.0
to serve the json content from the Play Controller. Angular's services would
call the RESTFul Play conrollers to consume the json response. This way there
is true separation of concerns - the UI and Server layer can be developed
independently and re-used.
        </p>

        <p>
            Integration of Angular JS with Play Framework is also very straightforward.
I've used the quick way and not sure whether this is the best way i.e. putting entire Angular app as part of <a href="http://www.playframework.org/documentation/2.0.2/Assets"> Play's Asset </a> folder.  
        </p>
        <hr>

        <h2>Step 0</h2>

        <p>
            Clone the Angular phonecat example from git as desribed
            <a href="http://docs.angularjs.org/tutorial">here</a>
            .
        </p>

        <p>Create a new Play 2.0 Java project</p>

        <h2>Step 1</h2>

        <p>
            Copy the entire example app - including app, config,logs,scripts,test directories to public directory of newly created Play application
        </p>

        <h2>Step 2</h2>

        <p>
            Write a service in Application Controller to serve the request.
            <script src="https://gist.github.com/3404689.js"></script>
        </p>

        <h2>Step 3</h2>

        <p>
            Add routes for the Play app in the  conf/routes file
            <script src="https://gist.github.com/3404695.js"></script>
             
        </p>
        <h2>Step 4</h2>
        <p>
            Change the build.sbt to add a dependency. I'm using Apache's commons io to do the file reading
            <script src="https://gist.github.com/3404699.js"></script>
        </p>

        <h2>Step 5</h2>
        <p>Run the app and navigate to http://localhost:9000</p>
        <hr>
        <p>The complete source code of this app is on Github. Clone/fork it - <a href="https://github.com/basav/momo"> https://github.com/basav/momo</a> </p>

    </div>
</div>

<div class="row">
    <div class="span3 columns">&nbsp;</div>
    <div class="span9 column">
            <p class="pull-right">{% if page.previous.url %} <a href="{{page.previous.url}}" title="Previous Post: {{page.previous.title}}"><i class="icon-chevron-left"></i></a>   {% endif %}   {% if page.next.url %}    <a href="{{page.next.url}}" title="Next Post: {{page.next.title}}"><i class="icon-chevron-right"></i></a>   {% endif %} </p>  
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