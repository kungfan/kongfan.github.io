---
layout: post
---

Github pages is a good place for hosting static blog on the internet, youcan
publish your web content on this platform for free.In addition to suporting
HTML,Github pages aslo support jekyll , a simple static site generator writing 
by ruby .It's a good choice for you to setup your blog by using jekyll .The
philosophy of jekyll is jekyll does what you want it to do , no more ,no less.
jekyll gets you out of your way and makes you focus on writing your blog .  
But just like many other static website or blog, the disadvantage of jekyll is 
blatantly obvious , the readers of your blog can't interact with your posts
because there is no comment function for your website .Thanks to the Disqus-a
blog comment system , it help us solve this problem elegantly .

now I'll show you how to add disqus to jekyll step by step. (**a memo for myself**)</br>
first of all , you need to creat a new file named disqus.html in _ includes 
directory and copy the "generic code" to this file . it look like this :
    
{% highlight html %}

<div id="disqus_thread"></div>
<script type="text/javascript">
    /* * *
     CONFIGURATION VARIABLES:
     EDIT BEFORE PASTING INTO YOUR WEBPAGE
    * * */

    /* * *
    required: replace example with your forum shortname
    * * */

    var disqus_shortname = 'kongfan';
    /* * * DON'T EDIT BELOW THIS LINE * * */
    (function() {
        var dsq = document.createElement('script'); 
        dsq.type = 'text/javascript';
        dsq.async = true;
        dsq.src = '//' + disqus_shortname + '.disqus.com/embed.js';
        (document.getElementsByTagName('head')[0] || 
        document.getElementsByTagName('body')[0]).appendChild(dsq);
    })();
</script>

{% endhighlight html %}    

and then , a html file named accout _ disqus should be created as well . typing
the follow code in this file :


{% highlight html %}
<script type="text/javascript">
/* * * CONFIGURATION VARIABLES: EDIT BEFORE PASTING INTO YOUR WEBPAGE * * */
/* * * required: replace example with your forum shortname * * */
var disqus_shortname = 'kongfan'; 

/* * * DON'T EDIT BELOW THIS LINE * * */
(function () {
    var s = document.createElement('script'); s.async = true;
    s.type = 'text/javascript';
    s.src = '//' + disqus_shortname + '.disqus.com/count.js';
    (document.getElementsByTagName('HEAD')[0] ||
     document.getElementsByTagName('BODY')[0]).appendChild(s);
    }());
</script>

{% endhighlight html %} 

In the third step , you need to know something about [liquid][1] and [yaml][2].
you can use include tag to add some code to   ~/ _  layout/post.html at the
bottom of this file. typing the code as follow : 



{% highlight html %}
---
layout: default
---
<h2>{{ page.title }}</h2>
<p class="meta">{{ page.date | date_to_string }}</p>

<div class="post">
{{ content }}
</div>
{ % include disqus_comment.html % }
{ % include count_comment.html % }
{% endhighlight html %}


[1]:http://liquidmarkup.org/
[2]:http://zh.wikipedia.org/zh-cn/YAML


