---
layout: default
---

<!-- Main jumbotron for a primary marketing message or call to action -->
<div class="jumbotron jumbo-dineroypolitica">  
  <div class="container">
    <h1>{{ site.title }}</h1>
    <p>{{site.description}}</p>
  </div>
</div>

<div class="container">
  {% include social-buttons.html %}

  {% include dineroypolitica/comparator.html %}
  {% include dineroypolitica/extrainfo.html %}

  {% include disqus.html %}
</div> <!-- cierra container -->