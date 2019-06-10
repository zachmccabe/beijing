---

layout: pek
pub-date: 2018-01-01
mod-date: 2018-02-02
title: test
image: https://www.zachmccabe.com/beijing/assets/viz/beijing-bonus-chapter-250.png
description: hello world
lede: aaaaa
cta: bbbbb

---


Some copy goes here. This is just some paragraph. Say something worth saying and say it right here.

{% include breadcrumbs.html %}

Do you see breadcrumbs?

---

Do you see the pages?

{% for page in site.pages %}
{% if page.url contains 'assets' or page.url contains '.xml' %}{% else %}
  <p>{{ page.url | replace: 'index.html', '' }}</p>
{% endif %}
{% endfor %}





---

Do you see the nav?

<nav>
  <p><a href="https://www.zachmccabe.com/beijing/faq.html" alt="FAQ">FAQ about this book</a></p>
  
  {% for page in site.pages %}
  {% if page.url contains '.xml' or page.url contains 'assets' or page.url contains 'bts' or page.url contains 'faq' %}{% else %}
    <p><a href="https://www.zachmccabe.com/beijing{{ page.url }}" alt="{{ page.title }}">{{ page.title }}</a></p>
  {% endif %}
  {% endfor %}
  
  <p><a href="#book-updates">Book updates</a></p>
  <hr />
  <p><a href="https://www.zachmccabe.com/beijing/how_the_book_got_made.html" alt="How the book got made">Behind the scenes: How the book got made</a></p>
</nav>
