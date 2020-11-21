---
layout: page
title: About
permalink: /about/
order: 99
---

Wir sind Teil der deutschsprachigen Java Community. Weil die JavaLand 2020 aufgrund der Corona-Pandemie abgesagt werden musste, haben wir die CyberLand als eine freie, virtuelle Konferenz ins Leben gerufen. Weitere Veranstaltungen sind nicht ausgeschlossen.


{% assign spaltenAnzahl = 4 %}
{% assign orga = site.data.orga %}

{% assign organizers = orga | where_exp:"orga", "orga.role == 'Organisator'" %}
{% assign ehemalige = orga | where_exp:"orga", "orga.role == 'Ehemalige'" %}
{% assign others = orga | where_exp:"orga", "orga.role != 'Organisator'" | where_exp:"orga", "orga.role != 'Ehemalige'" %}

### Organisatoren

{%- include elements/orga-grid.html organizers=organizers rows=4 -%}

### Ehemalige

{%- include elements/orga-grid.html organizers=ehemalige rows=4 -%}

### Helfer

{%- include elements/orga-grid.html organizers=others rows=4 -%}


{%- include elements/jugs.md -%}