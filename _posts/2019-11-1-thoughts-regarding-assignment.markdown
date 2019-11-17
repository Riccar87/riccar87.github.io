---
layout: post
comments: true
title:  "Thoughts regarding assignment"
date:   2019-11-17 12:34:11 -0100
categories: jekyll update
---

In the beginning of this assignment, I had a lot of issues with setting up Docker because I had Windows Home. Therefore I needed to get Windows Education but it took be almost a long time to get this to work because I had a lot of problems with getting the key. However, when I got the Windows education to work, the Docker installation went pretty smooth. I also got some problem when setting up Jekyll because `npm install` and `npm start` kept crashing so finally I needed to close all processes related to Docker and edit Docker settings to get it to work.

I really enjoyed working with the CSS preprocessor in this assignment. It felt a lot more fluid and I liked the all the possibilites with SASS that you can't get with pure CSS. For example I could write:

{% highlight ruby %}

$dark-background: #3A3A3E;
.site-header, .site-footer {
        background-color: $dark-background;
    }
{% endhighlight %}
Here I could assign both classes "site-header" and "-site-footer" the same background color without adding it twice, like:
{% highlight ruby %}
.site-header {
  background-color: #3A3A3E;
}
.site-footer {
    background-color: #3A3A3E;
}
{% endhighlight %}

As you can see, I also could use variable for the dark background color I wanted.
{% if page.comments %}
<div id="disqus_thread"></div>
<script>

/**
*  RECOMMENDED CONFIGURATION VARIABLES: EDIT AND UNCOMMENT THE SECTION BELOW TO INSERT DYNAMIC VALUES FROM YOUR PLATFORM OR CMS.
*  LEARN WHY DEFINING THESE VARIABLES IS IMPORTANT: https://disqus.com/admin/universalcode/#configuration-variables*/
/*
var disqus_config = function () {
this.page.url = PAGE_URL;  // Replace PAGE_URL with your page's canonical URL variable
this.page.identifier = PAGE_IDENTIFIER; // Replace PAGE_IDENTIFIER with your page's unique identifier variable
};
*/
(function() { // DON'T EDIT BELOW THIS LINE
var d = document, s = d.createElement('script');
s.src = 'https://riccar87.disqus.com/embed.js';
s.setAttribute('data-timestamp', +new Date());
(d.head || d.body).appendChild(s);
})();
</script>
<noscript>Please enable JavaScript to view the <a href="https://disqus.com/?ref_noscript">comments powered by Disqus.</a></noscript>    
{% endif %}
