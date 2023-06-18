---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
---

<h1><b>Zusammenfassung</b></h1>
<ul>
    {% for plant in site.plants %}
        <li>
            <h4><a href="{{ plant.url | relative_url }}">{{ plant.title }}</a></h4>
        </li>
    {% endfor %}
</ul>

<br>
<h1><b>Erfahrungsberichte</b></h1>
<ul>
    {% for protocol in site.experience %}
        <li>
            <h4>{{ protocol.title }}</h4>
            <p><a href="{{ protocol.url | relative_url }}">{{ protocol.year }}</a></p>
        </li>
    {% endfor %}
</ul>

<br>
<h1><b>Anleitung</b></h1>
<ul>
    {% for instruction in site.guide %}
        <li>
            <h4><a href="{{ instruction.url | relative_url }}">{{ instruction.title }}</a></h4>
        </li>
    {% endfor %}
</ul>
