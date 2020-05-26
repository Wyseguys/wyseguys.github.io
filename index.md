---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: default
---

<div class="home">
  <h1 class="page-heading">My Stupid Site On the Dumbernet</h1>
  <p>
  What is more important.  Putting my opinion on the internet or finding a cheap hosting solution and practice on SASS from time to time.</p>
  <hr />
  <h2 class="page-heading">Blag Posts</h2>
  <div class="row marketing">
      {% for post in site.posts limit:3 %}
      <div class="col-lg-4">
        {% assign date_format = site.minima.date_format | default: "%b %-d, %Y" %}
        <span class="post-meta">{{ post.date | date: date_format }}</span>
        <h3>
          <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
        </h3>
        <p>{{ post.excerpt }}</p>
      </div>
    {% endfor %}
  </div>
  <div class="row">
    <div class="col-lg-12">
        <h5 class="text-right"><a class="page-link" href="{{ site.baseurl }}{% link blag/index.html %}">Read the rest of Blag</a></h5>
    </div>
  </div>
  <div class="row">
    <div class="col-lg-12">
      <p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | relative_url }}">via RSS</a></p>
    </div>
  </div>
</div>