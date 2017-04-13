---
layout: page
---

I'm currently a postdoctoral scholar at the University of Kentucky and a philosophy instructor at Asbury University. 

My research puts an Aristotelian form of virtue ethics in conversation with contemporary ethical and metaphysical naturalism. For example, I'm especially interested in critiques of modern moral philosophy and the attempt to provide a scientifically respectable articulation of the age-old view that virtue is 'natural.'  More broadly, I have a long-standing interest in metaphysics and the philosophy of mind, Plato, and philosophy of religion. 

I completed my PhD in philosophy under the direction of David Bradshaw. I also hold a master's degree in Orthodox Theology from the University of Balamand and a bachelor's in Humanities from Biola University.
 


<br>

# Testimonials

- "A good-conversation machine." -- [Andrew Selby, Trinity Classical Academy](https://baylor.academia.edu/AndrewSelby)

* "Makes philosophy come alive..." -- [Chris Bounds, Asbury University](https://www.asbury.edu/academics/departments/christian-studies-philosophy/faculty-staff/chris-bounds)

*  "Dynamism, acumen, and compassion..."   -- [Peter Gross, Wheatstone Academy](http://www.wheatstoneministries.com/people/)

* "Enthusiastic and personable... clear and precise" -- [Dan Breazeale, University of Kentucky](https://philosophy.as.uky.edu/users/breazeal)

* "Give[s] me great hope for our next generation." -- [Cinda Tribble, Institute for Excellence in Writing](http://iew.com/cinda-tribble)


<br>






<div id="content" class="content">
    <h3>Recent Posts</h3>
    <ul class="category recent-posts">       
        {% for post in site.posts limit:3  %}
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
    </div>

