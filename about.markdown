---
layout: page
title: About
permalink: /about/
---

This is the base Jekyll theme. You can find out more info about customizing your Jekyll theme, as well as basic Jekyll usage documentation at [jekyllrb.com](https://jekyllrb.com/)

You can find the source code for Minima at GitHub:
[jekyll][jekyll-organization] /
[minima](https://github.com/jekyll/minima)

You can find the source code for Jekyll at GitHub:
[jekyll][jekyll-organization] /
[jekyll](https://github.com/jekyll/jekyll)


[jekyll-organization]: https://github.com/jekyll


<nav>
  <ul>
    {% assign nav_pages = site.pages | sort: "nav_order" %}
    {% for p in nav_pages %}
      {% if p.title %}
        <li>
          <a href="{{ p.url | relative_url }}" 
             class="{% if page.url == p.url %}active{% endif %}">
             {{ p.title }}
          </a>
        </li>
      {% endif %}
    {% endfor %}
  </ul>
</nav>
