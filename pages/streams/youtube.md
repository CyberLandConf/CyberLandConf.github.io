---
layout: default
number: 100
room: Youtube Stream CyberLand
youtubeId: ONfl-yp36DI
permalink: /stream/youtube
---

<div class="section">
    <div class="container session-details">
        <h1 class="room-title">{{ page.room }}</h1>
        <div>
            <iframe width="1280" height="720" src="https://www.youtube.com/embed/{{ page.youtubeId }}" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
        </div>
        Direkter Link zum <a href=" https://youtu.be/{{ page.youtubeId }}">Video-Stream</a>
    </div>
</div>



