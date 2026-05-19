---
layout: default
---

<script>
if (window.innerWidth <= 768) {
  window.location.replace("/titles");
}
</script>

<style>

.page-wrap {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 60px 40px;
  box-sizing: border-box;
  font-family: sans-serif;
  gap: 60px;
}

.site-header {
  cursor: pointer;
  width: 600px;
  max-width: 100%;
}

.site-header span {
  font-size: 70px;
  color: #111;
}

.main-img {
  width: 600px;
  height: auto;
  display: block;
  margin-top: 40px;
}

.bottom-row {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 600px;
}

.bottom-row a {
  font-size: 30px;
  text-decoration: none;
  color: #111;
  white-space: nowrap;
  transition: color 0.3s ease;
}

.bottom-row a:hover {
  color: #888;
}

.get-in-touch a {
  display: inline-block;
  text-decoration: none;
  color: #111;
  transition: color 0.3s ease;
}

/* GET IN TOUCH */

.get-in-touch {
  position: fixed;
  bottom: 80px;
  right: 100px;
  font-size: 14px;
  text-align: right;
  z-index: 200;
}

.get-in-touch a {
  text-decoration: none;
  color: #111;
  transition: color 0.3s ease;
}

.get-in-touch a:hover {
  color: #888;
}

/* © */

.copy {
  position: fixed;
  bottom: 60px;
  right: 100px;
  font-size: 14px;
  color: #111;
  text-align: right;
  font-family: sans-serif;
}

.meta-note {
  position: fixed;
  bottom: 40px;
  right: 100px;
  font-size: 14px;
  text-align: right;
  width: 260px;
  font-family: sans-serif;
  color: #111;
}

/* Mac */

@media (min-width: 769px) {

  .get-in-touch {
    font-size: 16px;
  }

}

/* 高さが低いとき（iPad横など） */

@media (max-height: 700px) {

  .copy {
    bottom: 50px;
  }

  .meta-note {
    bottom: 20px;
  }

}

/* オーバーレイ */

.overlay {
  display: none;
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(255,255,255,0.95);
  flex-direction: column;
  justify-content: center;
  align-items: center;
  z-index: 100;
  cursor: pointer;
  gap: 30px;
}

.overlay img {
  width: 480px;
  height: auto;
  max-width: 90vw;
  object-fit: contain;
}

.overlay .close-hint {
  font-size: 16px;
  color: #888;
  font-family: sans-serif;
}

</style>

<div class="page-wrap">

<div class="site-header" onclick="showOverlay()">
  <span>Je'm</span>
</div>

<img class="main-img" src="{{ '/jem3.jpg' | relative_url }}">

<div class="bottom-row">
  <a href="{{ '/titles' | relative_url }}">LYRICS</a>
  <a href="https://music.apple.com/jp/artist/jem/1864719862?l=en-US" target="_blank">APPLE MUSIC</a>
  <a href="https://jemmusicja.bandcamp.com" target="_blank">BANDCAMP</a>
</div>

</div>

<div class="get-in-touch">
  <a href="mailto:jemmusicja@duck.com">GET IN TOUCH</a>
</div>

<div class="copy">
Lyrics | Songs | Images
© 2024 All rights reserved
</div>

<div class="meta-note">
Designed for Mac and PC
</div>

<div class="overlay" id="overlay" onclick="hideOverlay()">
  <img src="{{ '/hime01.jpg' | relative_url }}">
  <div class="close-hint">CLICK TO CLOSE</div>
</div>

<script>

function showOverlay() {
  const overlay = document.getElementById('overlay');
  overlay.style.display = 'flex';
}

function hideOverlay() {
  const overlay = document.getElementById('overlay');
  overlay.style.display = 'none';
}

</script>
