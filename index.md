---
layout: page
title: 
no_link_title: false 
no_excerpt: false 
hide_image: false
cover: true
---

## HNR2027

The 12th International Historical Network Research Conference (HNR2027) will take place on **July 14th - 16th, 2027** at the Universidad Autónoma de San Luis Potosí in San Luis Potosí, SLP, Mexico. It brings together researchers applying network research methods across all the historical sciences, and strengthening an international community that grows, connects, and reaches an ever-wider audience.

<div style="display:flex; gap:2rem; align-items:center; flex-wrap:wrap;">
  <img src="img/hnr_logo_vector.png" width="200">
  <img src="{{ '/img/cintillo_logos.png' | relative_url }}" alt="UASLP, FHAB and IF LEDS" style="height:90px; width:auto">
</div>

## Important dates

| Milestone | Date |
|---|---|
| Call for papers | August 17th, 2026 |
| Deadline for submissions | December 11th, 2026 |
| Notification of acceptance | February 3rd, 2027 |
| Registration opening | March 3rd, 2027 |
| Conference | July 14th-16th, 2027 |

## Welcome

<div class="welcome-video">
  <div class="welcome-video__buttons" role="group" aria-label="Language selector">
    <button type="button" class="welcome-video__btn is-active" data-lang="en" data-id="PjSHZ-Lq37Q" onclick="switchWelcomeVideo(this)">Eng.</button>
    <button type="button" class="welcome-video__btn" data-lang="es" data-id="bK_0NH-vejo" onclick="switchWelcomeVideo(this)">Spa.</button>
  </div>
  <div class="welcome-video__frame">
    <iframe id="welcome-video-iframe"
      src="https://www.youtube-nocookie.com/embed/PjSHZ-Lq37Q"
      title="HNR2027 welcome video" frameborder="0"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
      allowfullscreen></iframe>
  </div>
</div>

<style>
.welcome-video__buttons { display:flex; gap:.5rem; margin-bottom:.75rem; }
.welcome-video__btn {
  cursor:pointer; padding:.35rem 1rem; border-radius:4px;
  border:1px solid var(--accent-color, #eacb76); background:transparent;
  color:inherit; font: inherit; font-size:.9rem; line-height:1;
}
.welcome-video__btn.is-active {
  background: var(--accent-color, #eacb76); color:#fff; font-weight:600;
}
.welcome-video__frame {
  position:relative; padding-bottom:56.25%; height:0; overflow:hidden;
  border-radius:6px;
}
.welcome-video__frame iframe {
  position:absolute; top:0; left:0; width:100%; height:100%; border:0;
}
</style>

<script>
function switchWelcomeVideo(btn) {
  var iframe = document.getElementById('welcome-video-iframe');
  iframe.src = 'https://www.youtube-nocookie.com/embed/' + btn.dataset.id;
  var buttons = btn.parentNode.querySelectorAll('.welcome-video__btn');
  for (var i = 0; i < buttons.length; i++) buttons[i].classList.remove('is-active');
  btn.classList.add('is-active');
}
</script>
