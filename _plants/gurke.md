---
layout: page
title: Gurke
plant: Gurke
permalink: /gurke
image: /experience/images/gurke/02-06-2023_erste_fruechte.jpeg
---


## __Sorte__

| Kiepenkerl Salatgurke    | Freilandgurke |
| -----------------------  | ------------  |
| ![]({{ '/experience/images/gurke/Sorte_Tanja.jpeg' | relative_url }}){: width="300" } | ![]({{ '/experience/images/gurke/Sorte_Freilandgurke.jpeg' | relative_url }}){: width="300" }
| Gattung: Tanja | Gattung: Cucumus sativus |
| Obi, Saatgut: 2,99€ | Dehner |
| Saatmenge: ca. 40 Stück | gekaufte Pflanze |
| Fazit: naja (zu große Kerne) | lecker

<hr>

## __Vorkultur__
Ab April können Gurken drinnen vorkultiviert werden. 
Ab Ende April können sie draußen abgehärtet werden (bei <6° reinholen)

### Saattiefe
- Samen hochkant in kleine Anzuchttöpfe  
- 1,5cm mit Erde bedecken 

<hr>

## __Auspflanzen__
1. Pflanze ohne Topf in Wasser bis keine Luftblasen mehr aufsteigen
2. Boden auflockern & glatt harken
3. Loch größer als Wurzelballen graben
4. Oberkante Wurzelballen mit Erdoberkante auf gleicher Höhe

### Zeitpunkt
Nach Eisheiligen

### Abstand
50cm

### Erde
TODO

### Zehrer 
Starkzehrer

### Standort
windgeschützt und sonnig


### Nachbarn

| gute Nachbarn | schlechte Nachbarn | 
| ------------- |:------------------:| 
| Basilikum     | Tomaten            |
| Dill          | Kürbis             |
|               | Zucchini           |


<hr>

## __Gießen__
- Mit lau- oder umgebungswarmen Wasser gießen, am Besten Regenwasser (sonst werden Gurken bitter)
- Sie sind Flachwurzler, weshalb sie sehr viel Wasser benötigen
- Lieber morgens statt abends gießen (von unten gießen, mögen kein Wasser auf den Blättern)

### Gießring
Eine Vertiefung von 0,5cm und eine Mauer von 1cm um die Pfanze anlegen

<hr>

## __Pflege__

### Düngen
TODO

### Rankhilfe
Je nach Sorte können Gurken z.B. vom Hochbeet runter wachsen oder benötigten eine Rankhilfe zum nach oben wachsen

Der Nachteil wenn sie am Hochbeet runterwachsen, ist das die Gurken auf der Seite wo sie am Hochbeet liegen weniger grün werden. Demzufolge hat die Gurke keine gleichmäßig dunkel-grün Farbe.

### Krumme Gurke
Mögliche Ursachen:
- zu wenig Wasser (Sobald sich Früchte entwickeln sollte die Gurke reichlich mit Wasser versorgt werden)
- zu starke Sonneneinstrahlung (Sehr heiße Temperaturen halten die Bestäuber fern und töten sogar den Pollen ab, so dass er steril bleibt)
- die Zugabe von zu viel Stickstoffdünger 

<hr>

## __Schädlinge__

### Mehltau 
TODO

### Sonnenbrand
TODO

### Schnecken
TODO

## __Ernte__
Am Stiel in der Mitte abschneiden, nicht abreißen!

### Merkmale
Wenn Schale glatt, gleichmäßig gefärbt und das Ende stumpf ist. 
Wird die Gurke mit einer Länge von 20-30cm geenrtet, regt das zu einem stärkere Wachstum und somit zu einer größeren Ernte an.

### Tageszeit
Die beste Tageszeit zum Ernten ist morgens, da die Gurken über den Tage an Wasser verlieren. Sie sind dann knackiger und länger haltbar.

### Lagern
TODO

<br>
<hr>
<hr>

### Verzeichnis

<ul class="list">
    {% for experience in site.experience %}
        {% if experience.plant contains page.plant %}
            <li>
                <a href="{{ experience.url | relative_url }}">{{ experience.year }}</a>
            </li>
        {% endif %}
    {% endfor %}
</ul>
