---
layout: default
---
{% include JB/setup %}


<ul class="posts">
  {% for post in site.posts %}
    <li>
      <h4>
        <a href="{{ BASE_PATH }}{{ post.url }}">{{post.title}}</a>
        <small>{{ post.date | date_to_long_string}}</small>
      </h4>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>


