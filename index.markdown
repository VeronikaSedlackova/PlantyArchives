---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
---

<h1>Meine Pflanzen</h1>

<ul>
    {% for plant in site.plants %}
        <li>
            <h2><a href="{{ plant.url | relative_url }}">{{ plant.title }}</a></h2>
            {% if plant.image %}
            <img src="{{ site.baseurl }}/plants/{{ plant.image }}">

            {% endif %}
            <p>{{ plant.summary | markdownify }}</p>
        </li>
    {% endfor %}

</ul>
