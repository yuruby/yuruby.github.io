---
layout: page
title: ゆるびぃ会
tagline: 
---
{% include JB/setup %}

## ゆるびぃ会とは

<hr>

作成途中...




<a href="{{ site.github_url }}" target="_blank"><img src="img/github_icon.png">{{ site.author.github }}</a>

<a href="{{ site.facebook_url }}" target="_blank"><img src="img/facebook_icon.png">{{ site.author.facebook }}</a>

<a href='http://cloud.feedly.com/#subscription%2Ffeed%2Fhttp%3A%2F%2Fyuruby.github.io%2Fatom.xml'  target='blank'><img id='feedlyFollow' src='http://s3.feedly.com/img/follows/feedly-follow-rectangle-flat-big_2x.png' alt='follow us in feedly' width='131' height='56'></a>


## New Post

<hr>

{% for post in site.posts limit:1 %}
  <div class="new_post">
    <h3>
        <span class="date">{{ post.date　| date: "%B %e, %Y"}}</span> &raquo;  <a href="{{ post.url }}">{{ post.title }}</a> - <a href="{{ post.author_url }}" target="_blank">{{ post.author }}</a>
    </h3>
    <div>{{ post.content }} </div>
  </div>
{% endfor %}