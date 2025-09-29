---
layout: default
title: Home
---
<div class="home">
    <div class="site-cover">
        <img src="/assets/images/footerInstagram.jpg" alt="Portada del blog">
        <h1 class="site-cover-title">Bienvenidos a Hornazos por el Mundo</h1>
    </div>

    <h2 class="post-list-heading">Recetas Recientes</h2>
    <ul class="post-list">
        {% for post in site.posts %}
        <li>
            <span class="post-meta">{{ post.date | date: "%-d %b %Y" }}</span>
            <h3>
                <a class="post-link" href="{{ post.url | relative_url }}">
                    {{ post.title | escape }}
                </a>
            </h3>
            <p>{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
        </li>
        {% endfor %}
    </ul>

    <p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | relative_url }}">via RSS</a></p>
</div>