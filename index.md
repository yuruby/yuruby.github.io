---
layout: page
title: ゆるびぃ会
tagline:
---
{% include JB/setup %}


<a href="{{ site.slackin_url }}"  target="_blank"><img src="img/slack.png"> Slack 使ってます。Slackinを用意してますので、こちらから参加できます。</a>

{% for post in site.posts limit:5 %}
  <div class="new_post">
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <div class="post-header">
      <span class="date">{{ post.date | date: "%Y年%m月%e日"}} </span>
      <span class="author">
        / 書いた人: <a href="{{ post.author_url }}" target="_blank">{{ post.author }}</a>
      </span>
    </div>
    <div>{{ post.content }}</div>
    <hr>
  </div>
{% endfor %}

<div class="footer">
  <a href="{{ site.github_url }}" target="_blank"><img src="img/github_icon.png"></a>
  <a href="{{ site.facebook_url }}" target="_blank"><img src="img/facebook_icon.png"></a>
  <a href='http://cloud.feedly.com/#subscription%2Ffeed%2Fhttp%3A%2F%2Fyuruby.github.io%2Fatom.xml'  target='blank'><img id='feedlyFollow' src='http://s3.feedly.com/img/follows/feedly-follow-rectangle-flat-big_2x.png' alt='follow us in feedly' width='131' height='56'></a>
</div>
