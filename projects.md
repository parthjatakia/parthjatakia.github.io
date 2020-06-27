---
layout: page
title: Projects
permalink: /projects/
---

<!--<div id="gh-latest"></div>-->
<div class="posts">
  {% for post in site.posts %}
    {% if post.type == 'projects' %}
      <article class="post">

        <h1 style="text-align:left;"><span style="text-align:left"><a href="{{ site.baseurl }}{{ post.url }}" style="text-align:left;">{{ post.title }}</a></span></h1>

        <div>
          <p class="post_date" style="text-align:left;">{{ post.when }}</p>
        </div>

        <div class="entry">
          {{ post.summary }}
        </div>

      </article>
    {% endif %}
  {% endfor %}
</div>

