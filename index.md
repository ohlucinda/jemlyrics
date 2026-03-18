---
layout: default
---

<style>
.page-wrap {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding: 30px 40px;
  box-sizing: border-box;
  font-family: 'Aboreto', cursive;
  gap: 50px;
}

.site-header {
  margin-bottom: 20px;
  cursor: pointer;
}

.site-header span {
  font-size: 100px;
  color: inherit;
}

.wrapper {
  display: flex;
  align-items: center;
  gap: 80px;
}

.left {
  display: flex;
  flex-direction: column;
  gap: 40px;
}

.left a {
  font-size: 56px;
  text-decoration: none;
  color: inherit;
}

.right-col {
  display: flex;
  flex-direction: column;
  gap: 12px;
}

.right-col img {
  height: 70vh;
  width: auto;
  display: block;
}

.bottom {
  display: flex;
  flex-direction: column;
  align-items: flex-end;
  gap: 6px;
}

.bottom a {
  font-size: 32px;
  text-decoration: none;
  color: inherit;
}

.copy {
  font-size: 20px;
  margin-top: 4px;
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
  justify-content: center;
  align-items: center;
  z-index: 100;
  cursor: pointer;
}

.overlay img {
  max-height: 90vh;
  max-width: 90vw;
  object-fit: contain;
}

.overlay .close-hint {
  position: fixed;
  bottom: 40px;
  font-size: 20px;
  color: #888;
  font-family: 'Aboreto', cursive;
}
</style>

<div class="page-wrap">

  <div class="site-header" onclick="showOverlay()">
    <span>JE'M</span>
  </div>

  <div class="wrapper">
    <div class="left">
      <a href="https://ohlucinda.wixsite.com/jemmusicja" target="_blank">MY NAME IS JE'M</a>
      <a href="{{ '/lyrics' | relative_url }}">LYRICS</a>
      <a href="https://ohlucinda.wixsite.com/jemmusicja/blog" target="_blank">MY NOTES</a>
    </div>
    <div class="right-col">
      <img src="{{ '/jem.jpg' | relative_url }}">
      <div class="bottom">
        <a href="https://music.apple.com/jp/artist/jem/1864719862?l=en-US" target="_blank">APPLE MUSIC</a>
        <a href="https://www.youtube.com/@JEMMUSICJA" target="_blank">YOUTUBE</a>
        <div class="copy">© All rights reserved</div>
      </div>
    </div>
  </div>

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
