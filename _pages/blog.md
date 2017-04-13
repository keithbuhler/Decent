---
layout:    page
permalink: "/buhlerreport/"
author:    kbuhler
keywords:  blog buhler report
title:     Buhler Report
menutitle: Blog
weight:    85
excerpt:   Timeless wisdom. Current events.

---

<div id="content" class="content">
    <h3>Categories</h3>
    {% assign sorted_cats = site.categories | sort %}
    {% for category in sorted_cats %}
    {% assign sorted_posts = category[1] | reversed %}
    <h3 id="{{category[0] | uri_escape | downcase | slugify }}">{{category[0] | camelcase }}</h3>
    <ul class="category {{category[0] | uri_escape | downcase | slugify}}">  
        {% for post in sorted_posts %}
        {% unless post.draft %}

        {% if post.menutitle %}
        {% assign title = post.menutitle %}
        {% else %}
        {% assign title = post.title %}
        {% endif %}

        <li>
            <div class="article">
                <article class="article" itemscope itemtype="http://schema.org/BlogPosting">
                    <header class="post-header">
                        <span class="title"><a itemprop="name" href="{{ post.url | absolute_url }}" title="{{ title }}">{{ title }}</a></span>
                        <time class="date" itemprop="datePublished" datetime="{{post.date | date: "%Y-%m-%d"}}">{{post.date | date: "%B %e, %Y"}}</time>
                    </header>
                </article>
            </div>
        </li>
        {% endunless %}
        {% endfor %}
    </ul>
    {% endfor %}



</div>




<h3> About </h3>

*The Buhler Report aims to enlighten and entertain by publishing timeless wisdom and the latest news about academic philosophy, classical education, politics, and more. Your comments are read and appreciated. All opinions contained in this site are the author's alone and do not represent the views of any organizations he is affiliated with.*


<h3> Comment </h3>


![Buhler](http://www.keithbuhler.com/images/buhler-oxford.JPG)

If you read something you like, hate, or disagree with, share or post a comment and let's dialogue. 



<br>

<center>

<!-- Begin MailChimp Signup Form -->

<link href="//cdn-images.mailchimp.com/embedcode/horizontal-slim-10_7.css" rel="stylesheet" type="text/css">
<style type="text/css">
      #mc_embed_signup{background:#fff; clear:left; font:14px Helvetica,Arial,sans-serif; width:100%;}
      /* Add your own MailChimp form style overrides in your site stylesheet or in this style block.
         We recommend moving this block and the preceding CSS link to the HEAD of your HTML file. */
</style>
<div id="mc_embed_signup">
<form action="//keithbuhler.us1.list-manage.com/subscribe/post?u=97f6265af674b156b34528bd4&amp;id=22e9d219d4" method="post" id="mc-embedded-subscribe-form" name="mc-embedded-subscribe-form" class="validate" target="_blank" novalidate>
    <div id="mc_embed_signup_scroll">
      <label for="mce-EMAIL">Subscribe here</label>
      <input type="email" value="" name="EMAIL" class="email" id="mce-EMAIL" placeholder="email address" required>
    <!-- real people should not fill this in and expect good things - do not remove this or risk form bot signups-->
    <div style="position: absolute; left: -5000px;" aria-hidden="true"><input type="text" name="b_97f6265af674b156b34528bd4_22e9d219d4" tabindex="-1" value=""></div>
    <div class="clear"><input type="submit" value="Subscribe" name="subscribe" id="mc-embedded-subscribe" class="button"></div>
    </div>
</form>
</div>

<!--End mc_embed_signup-->

Thanks for reading. 


<br> 


<br><a href="https://www.freecounterstat.com">
</a><noscript><a href="https://www.freecounterstat.com" title="web counter"><img src="https://counter1.fcs.ovh/private/freecounterstat.php?c=x8gasubftx7e24qf671gwk2g3eqqtns2" border="0" title="web counter" alt="web counter"></a></noscript>

<br>

</center> 

<script type="text/javascript">require(["mojo/signup-forms/Loader"], function(L) { L.start({"baseUrl":"mc.us1.list-manage.com","uuid":"97f6265af674b156b34528bd4","lid":"22e9d219d4"}) })
</script>



<!-- Code for posting just an excerpt (with no image) of each post. Put under heading. {% if post.excerpt %}<p class="archive__item-excerpt" itemprop="description">{{ post.excerpt | markdownify | strip_html | truncate: 160 }}</p>{% endif %}-->


<script type="text/javascript" src="https://counter1.fcs.ovh/private/counter.js?c=x8gasubftx7e24qf671gwk2g3eqqtns2"></script>
