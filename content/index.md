---
title: Les aventures d'Elma
comments: false
---

Bienvenue sur le blog d'Elma !

Suivez nos aventures à bord d'[[Elma]] de la Bretagne jusqu'au Japon.

## [[Trajet | Carte de la trajectoire prévue]] :

<iframe class="fullwidth-map" src="/static/map.html" title="Route map"></iframe>


<div id="countdown" style="font-size:1.5rem; font-weight:600;">Loading…</div>
<script>
(function () {
  const target = new Date("2027-02-14T12:00:00"); // change this date
  let timer;
  function tick() {
    const el = document.getElementById("countdown");
    if (!el) { clearInterval(timer); return; }
    const diff = target - new Date();
    if (diff <= 0) { el.textContent = "C'est parti !"; clearInterval(timer); return; }
    const d = Math.floor(diff / 86400000);
    const h = Math.floor(diff / 3600000) % 24;
    const m = Math.floor(diff / 60000) % 60;
    const s = Math.floor(diff / 1000) % 60;
    el.textContent = `Départ dans ${d}j ${h}h ${m}m ${s}s !`;
  }
  function start() { clearInterval(timer); tick(); timer = setInterval(tick, 1000); }
  start();
  document.addEventListener("nav", start);
})();
</script>



## Ou est Elma ?

Tracking 1: NoForeignLand (Satellite + Terrestre)

<iframe
  class="route-map"
  title="NoForeignLand"
  src="https://www.noforeignland.com/map/embed/6755394716186934/5/on/day/"
  width="100%"
  height="500"
  style="border:0;"
></iframe>

Tracking 2: Marine Traffic (AIS, mmsi: 227446440)

<iframe
  class="route-map"
  title="Marine traffic"
  src="https://www.marinetraffic.com/en/ais/embed/zoom:3/centery:48/centerx:-5/maptype:4/shownames:false/mmsi:227446440/shipid:0/fleet:/fleet_id:/vtypes:/showmenu:/remember:false"
  width="100%"
  height="500"
  style="border:0;"
></iframe>

*Des interruptions du tracking de plusieurs heures ou jours sont possibles.*