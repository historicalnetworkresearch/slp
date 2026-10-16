---
layout: page
title: 
no_link_title: false 
no_excerpt: false 
hide_image: false
cover: true
---

{% include lang-switch.html %}

<div class="lang-content" data-lang="en" lang="en" markdown="1">

## HNR2027

The 12th International Historical Network Research Conference (HNR2027) will take place on **July 14th - 16th, 2027** at the Universidad Autónoma de San Luis Potosí in San Luis Potosí, SLP, Mexico. It brings together researchers applying network research methods across all the historical sciences, and strengthening an international community that grows, connects, and reaches an ever-wider audience.

<div style="display:flex; gap:2rem; align-items:center; flex-wrap:wrap;">
  <img src="{{ '/img/hnr_logo_vector.png' | relative_url }}" alt="Historical Network Research" width="200">
  <img src="{{ '/img/cintillo_logos.png' | relative_url }}" alt="UASLP, FHAB and IF LEDS" style="height:90px; width:auto">
</div>

## Important dates

| Milestone | Date |
|---|---|
{% for m in site.data.dates.milestones %}| {{ m.en.milestone }} | {{ m.en.date }} |
{% endfor %}

## Welcome

</div>

<div class="lang-content" data-lang="es" lang="es" markdown="1" style="display:none">

## HNR2027

La 12.ª Conferencia Internacional de Investigación de Redes Históricas (HNR2027) se celebrará del **14 al 16 de julio de 2027** en la Universidad Autónoma de San Luis Potosí, en San Luis Potosí, SLP, México. Reúne a investigadores que aplican métodos de análisis de redes en todas las ciencias históricas y fortalece una comunidad internacional que crece, se conecta y llega a un público cada vez más amplio.

<div style="display:flex; gap:2rem; align-items:center; flex-wrap:wrap;">
  <img src="{{ '/img/hnr_logo_vector.png' | relative_url }}" alt="Historical Network Research" width="200">
  <img src="{{ '/img/cintillo_logos.png' | relative_url }}" alt="UASLP, FHAB e IF LEDS" style="height:90px; width:auto">
</div>

## Fechas importantes

| Hito | Fecha |
|---|---|
{% for m in site.data.dates.milestones %}| {{ m.es.milestone }} | {{ m.es.date }} |
{% endfor %}

## Bienvenida

</div>

<!-- One shared player: its source follows the page language switch above. -->
<div class="welcome-video">
  <div class="welcome-video__frame">
    <iframe id="welcome-video-iframe"
      src="https://www.youtube-nocookie.com/embed/PjSHZ-Lq37Q"
      title="HNR2027 welcome video" frameborder="0"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
      allowfullscreen></iframe>
  </div>
</div>

<style>
.welcome-video__frame {
  position:relative; padding-bottom:56.25%; height:0; overflow:hidden;
  border-radius:6px;
}
.welcome-video__frame iframe {
  position:absolute; top:0; left:0; width:100%; height:100%; border:0;
}
</style>

<script>
(function () {
  var VIDEOS = { en: 'PjSHZ-Lq37Q', es: 'bK_0NH-vejo' };
  var TITLES = { en: 'HNR2027 welcome video', es: 'Video de bienvenida HNR2027' };

  document.addEventListener('langchange', function (event) {
    var lang = event.detail.lang;
    var iframe = document.getElementById('welcome-video-iframe');
    if (!iframe || !VIDEOS[lang]) return;
    var next = 'https://www.youtube-nocookie.com/embed/' + VIDEOS[lang];
    if (iframe.src !== next) iframe.src = next;
    iframe.title = TITLES[lang];
  });
})();
</script>
