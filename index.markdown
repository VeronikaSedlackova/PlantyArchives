---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
---

<style>
    .grid {
        display: grid;
        grid-template-columns: 1fr 1fr;
        gap: 1rem;
    }
    ul.grid {
        margin: 0;
        list-style: none;
    }
    .list {
        display: flex;
        gap: 1rem;
    }
    ul.list {
        margin: 0;
        list-style: none;
    }
    .entry {
        display: grid;
        place-items: center;
    }
    .image-tile {
        object-fit: cover;
        border-radius: 1rem;
        overflow: hidden;
        height: 10rem;
        width: 100%;
    }
</style>

<h1><b>Zusammenfassung</b></h1>
<ul class="grid">
    {% for plant in site.plants %}
        <li class="entry">
            <img class="image-tile" src="{{ plant.image | relative_url }}" alt="{{ plant.title }}">
            <h4><a href="{{ plant.url | relative_url }}">{{ plant.title }}</a></h4>
            <ul class="list">
                {% for experience in site.experience %}
                {% if experience.plant contains plant.plant %}
                    <li>
                        <h4><a href="{{ experience.url | relative_url }}">{{ experience.year }}</a></h4>
                    </li>
                {% endif %}
                {% endfor %}
            </ul>
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

<br>
<h1><b>Utensilien</b></h1>
<ul>
    {% for utensils in site.equipment %}
        <li>
            <h4><a href="{{ utensils.url | relative_url }}">{{ utensils.title }}</a></h4>
        </li>
    {% endfor %}
</ul>

<br>
<h1><b>Roadmap</b></h1>
<ul>
    {% for map in site.roadmap %}
        <li>
            <h4><a href="{{ map.url | relative_url }}">{{ map.title }}</a></h4>
        </li>
    {% endfor %}
</ul>
