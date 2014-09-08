---
layout: default
---

<!-- Main jumbotron for a primary marketing message or call to action -->
<div class="jumbotron jumbo-binominal">  
  <div class="container">
    <h1>¿Hay acuerdo?</h1>
    <h3>La Reforma al Sistema Binominal cambiará la forma en que elegimos a nuestros parlamentarios. Infórmate sobre los puntos de vista de diversos actores sociales con respecto a las posturas del Gobierno. Elige un actor y compara sus posiciones.</h3>
  </div>
</div>

<div class="container">
  {% include social-buttons.html %}

  {% include binominal/comparator.html %}

  {% include binominal/extrainfo.html %}
  {% include disqus.html %}
</div> <!-- cierra container -->

{% include footer.html %}