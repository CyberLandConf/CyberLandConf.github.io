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
        <div>
            <iframe width="80%" height="100%" src="https://www.youtube.com/embed/{{ page.youtubeId }}" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
            <!--iframe id="dynamicIframe" style="overflow:hidden;overflow-x:hidden;overflow-y:hidden;height:100%;width:80%;position:absolute;top:0px;left:0px;right:0px;bottom:0px" height="100%" width="100%" src="https://www.youtube.com/embed/ctixIsKwigo?si=MihCKCgPYMGc0_XG" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe -->
            <iframe style="height:100%;width:20%;right:0px;top:0px;" src="https://www.youtube.com/live_chat?v={{ page.youtubeId }}&embed_domain=cyberland.ijug.eu" ></iframe>
        </div>
        Direkter Link zum <a href=" https://youtu.be/{{ page.youtubeId }}">Video-Stream</a>
    </div>
</div>
