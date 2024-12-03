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
        <div style="height:90vh">
            <iframe style="overflow:hidden;overflow-x:hidden;overflow-y:hidden;height:70vh;width:100%;position:absolute;left:0px;right:0px;top:0px" src="https://www.youtube.com/embed/{{ page.youtubeId }}" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
            <iframe style="overflow:hidden;overflow-x:hidden;overflow-y:hidden;height:20vh;width:100%;position:absolute;left:0px;right:0px;bottom:0px" src="https://www.youtube.com/live_chat?v={{ page.youtubeId }}&embed_domain=cyberland.ijug.eu" ></iframe>
        </div>
    </div>
    Direkter Link zum <a href=" https://youtu.be/{{ page.youtubeId }}">Video-Stream</a>

</div>
