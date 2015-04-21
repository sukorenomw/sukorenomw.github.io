---
layout: page
permalink: /about/index.html
title: Sukoreno Mukti Widodo
tags: [sukoreno, mukti, widodo]
---

<figure>
  <img src="{{ site.url }}/images/hmfaysal.jpg" alt="Sukoreno Mukti Widodo">
  <figcaption>Sukoreno Mukti Widodo</figcaption>
</figure>

{% assign total_words = 0 %}
{% assign total_readtime = 0 %}
{% assign featuredcount = 0 %}
{% assign statuscount = 0 %}

{% for post in site.posts %}
    {% assign post_words = post.content | strip_html | number_of_words %}
    {% assign readtime = post_words | append: '.0' | divided_by:200 %}
    {% assign total_words = total_words | plus: post_words %}
    {% assign total_readtime = total_readtime | plus: readtime %}
    {% if post.featured %}
    {% assign featuredcount = featuredcount | plus: 1 %}
    {% endif %}
{% endfor %}


My name is **Sukoreno Mukti Widodo**, and this is my personal blog. Studied Informatics Engineering at Institut Teknologi Harapan Bangsa, Bandung, Indonesia.
I am passionate about developing web based application using databases (Oracle, MySQL), PHP programming language with CodeIgniter Framework, currently working on Multi Theft Auto GTA SA game server with average 90 player per day, i also joined ubuntu launchpad team, ubuntu indonesian team and currently marked for bug management

### More Information
Currently working on Indolife Game Portal as a Web Developer and Game scripter, you can visit [Indolife Game Portal](http://www.indoliferoleplay.com "Indolife's Homepage") for more info about Indolife Game Portal 

### Contact me

[sukorenomw@gmail.com](mailto:email@domain.com)