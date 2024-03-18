---
layout: page
title: About
permalink: /about/
order: 99
---

Wir sind Teil der deutschsprachigen Java Community. Weil die JavaLand 2020 aufgrund der Corona-Pandemie abgesagt werden musste, haben wir die CyberLand als eine freie, virtuelle Konferenz ins Leben gerufen und innerhalb weniger Tage organisiert. Die erste Durchführung war ein voller Erfolg. Mittlerweile führen wir regelmässig verschiedene Online-Formate durch.


{% assign spaltenAnzahl = 3 %}
{% assign orga = site.data.orga %}

{% assign organizers = orga | where_exp:"orga", "orga.role == 'Organisator'" %}
{% assign ehemalige = orga | where_exp:"orga", "orga.role == 'Ehemalige'" %}
{% assign others = orga | where_exp:"orga", "orga.role != 'Organisator'" | where_exp:"orga", "orga.role != 'Ehemalige'" %}

### Organisatoren

{%- include elements/orga-grid.html organizers=organizers rows=spaltenAnzahl -%}

### Ehemalige

{%- include elements/orga-grid.html organizers=ehemalige rows=spaltenAnzahl -%}

### Helfer

{%- include elements/orga-grid.html organizers=others rows=spaltenAnzahl -%}

{%- include elements/usergroups.html -%}

### Sponsoren

{%- include elements/sponsors.html -%}
