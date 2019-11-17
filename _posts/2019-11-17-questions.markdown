---
layout: post
comments: true
title:  "Q&A"
date:   2019-11-17 1:10:11 -0600
categories: jekyll update
---

## QnA with Rickard
Today I'm going to answer some questions that I've been asked. Here's my answers!

* What do you think of pre-compiling your CSS?

`Very useful`
* What do you think of static site generators?

`Very useful for smaller STATIC projects. Its a good choice for when you have a need to relay information to a group of people without needing any user interactions.`
`Suitable projects could be smaller fraternities or other smaller groups`
* What is robots.txt and how have you configure it for your site?

`robots.txt is for instructions for bots. I configured it in a way so that they would not scan my site. I added it on root.`
* What is humans.txt and how have you configure it for your site?

`humans.txt is a place where you can credit authors and peole who assisted you in developing the website. I added my own name and information in the root.`

* How did you implements comments to blog posts

`I havent yet`
* What is Open Graph and how do you make use of it?

`Its to make links more interesting. So that theres a little tid-bit of information/picture along with the link.`

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