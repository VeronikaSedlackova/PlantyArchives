---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
---

<h1>Meine Pflanzen</h1>

<ul>
    {% for plant in site.plants %}
        <li>
            <h2>{{ plant.title }}</h2>
            <p><a href="{{ plant.url | relative_url }}">Übersicht</a></p>
            <h3>{{ plant.year }}</h3>
            {% if plant.image %}
            <img src="{{ plant.image | relative_url }}">

            {% endif %}
            <p>{{ plant.summary | markdownify }}</p>
        </li>
    {% endfor %}

</ul>
