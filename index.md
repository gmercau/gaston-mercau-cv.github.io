---
layout: default
title: Mi CV Profesional
---

{% raw %}
<h1>{{ site.data.cv.nombre }}</h1>
<h2>{{ site.data.cv.profesion }}</h2>

<h3>Experiencia</h3>
<ul>
  {% for exp in site.data.cv.experiencia %}
    <li>
      <strong>{{ exp.puesto }}</strong> en {{ exp.empresa }} ({{ exp.periodo }})
      <ul>
        {% for logro in exp.logros %}
          <li>{{ logro }}</li>
        {% endfor %}
      </ul>
    </li>
  {% endfor %}
</ul>
{% endraw %}
