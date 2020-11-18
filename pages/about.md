---
layout: page
title: About
permalink: /about/
order: 99
---

Wir sind Teil der deutschsprachigen Java Community. Weil die JavaLand 2020 aufgrund der Corona-Pandemie abgesagt werden musste, haben wir die CyberLand als eine freie, virtuelle Konferenz ins Leben gerufen. Weitere Veranstaltungen sind nicht ausgeschlossen.


{% assign spaltenAnzahl = 4 %}
{% assign organizers = site.data.orga %}

<div class="speaker-grid">
    <div class="columns">
{% for member in organizers %}
  {% assign istLetzteZelle = forloop.index | modulo: 4 %}
        <div class="column">{%- include elements/orga-info.html member=member -%}</div>
  {% if istLetzteZelle == 0 %}
    </div>
    <div class="columns">
  {% endif %}
{% endfor %}
{% assign zellenLetzteZeile = organizers.size | modulo: spaltenAnzahl %}
{% assign leereZellen = spaltenAnzahl | minus: zellenLetzteZeile %}
{% for i in (1..leereZellen) %}
        <div class="column"></div>
{% endfor %}
    </div>
</div>