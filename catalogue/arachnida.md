---
layout: default
title: arachnid catalogue
categories: photography arachnida
---

# Arachnida

Spiders (order Araneae) are the best-known members of class Arachnida, and many
people know scorpions (order Scorpiones) are also arachnids, but in fact there
are several smaller, more obscure orders included in this class. These creatures
tend to be rarer, and I only have a few photos of them.

  {% for page in site.arachnida %}
  <a href="{{page.url}}">{{ page.heading }}</a>
  {% endfor %}
