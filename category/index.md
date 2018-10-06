---
layout: page
---
<div class="row">
    <div class="col-lg-12">
        <h1>Blag Cotegories</h1>
    </div>
</div>
<div class="row">
    <div class="col-lg-6">
        <p>Like any good personal who is egomanical to post their crap on the Internet, I have taken the time to organize and apply metadata.  Lets use this metadata together to find the topic you want.</p>
        <p>If you don't see what you are looking for, maybe you are not looking in the right place.  I mean, you read the shitty roommate story, so what else is on here.  I am not funny, Martin was funny.</p>
    </div>
    <div class="col-lg-6">
        {% for category in site.categories %}
        <h3>{{ category[0] }}</h3>
        <ol>
            {% for post in category[1] limit:3 %}
            <li><a href="{{ post.url }}">{{ post.title }}</a></li>
            {% endfor %}
        </ol>
        {% endfor %}
    </div>
</div>
