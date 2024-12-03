---
layout: default
number: 100
room: Youtube Stream 1 CyberLand Ladies Night 04.12.24
youtubeId: ctixIsKwigo
permalink: /stream/1
---

<div class="section">
    <div class="container session-details">
        <h1 class="room-title">{{ page.room }}</h1>
        <div style="height:80vh">
            <iframe style="width:100%;aspect-ratio: 16 / 9;" src="https://www.youtube.com/embed/{{ page.youtubeId }}" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe><br/>
            <iframe style="width:100%;height:40vh" src="https://www.youtube.com/live_chat?v={{ page.youtubeId }}&embed_domain=cyberland.ijug.eu" ></iframe>
        </div><br/>
        Direkter Link zum <a href=" https://youtu.be/{{ page.youtubeId }}">Video-Stream</a>
    </div>

</div>
