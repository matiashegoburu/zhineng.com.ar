---
layout: page
show_meta: false
title: "Actividades"
teaser: "Estas son nuestras actividades, ¡te invitamos a que participes!"
header:
   image_fullwidth: "homeHeader.png"
permalink: "/actividades/"
---
{% assign pages = site.pages | where:"layout","actividad" %}

<div>
  <ul class="small-block-grid-3">
{% for page in pages %}
  <li style="text-align: center;"><a href="{{ page.url }}"><img src="{{ site.url }}{{ site.baseurl }}/assets/img/actividades/{{page.actividad}}/{{ page.gallery-image }}" />{{ page.title }}</a></li>
{% endfor %}
  </ul>
</div>

{% include dudas-general-widget %}
</script>
