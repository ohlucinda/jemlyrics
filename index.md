---
layout: default
---

<style>
.page-wrap {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 60px 40px;
  box-sizing: border-box;
  font-family: 'Aboreto', cursive;
  gap: 40px;
}

.site-header {
  cursor: pointer;
}

.site-header span {
  font-size: 70px;
  color: inherit;
}

.main-img {
  width: 560px;
  height: auto;
  display: block;
}

.bottom-row {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 560px;
  gap: 40px;
}

.bottom-row a {
  font-size: 24px;
  text-decoration: none;
  color: inherit;
  white-space: nowrap;
}

.copy {
  font-size: 14px;
  white-space: nowrap;
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
  font-family: 'Aboreto', cursive;
}

/* スマホ用 */
@media (max-width: 768px) {
  .page-wrap {
    padding: 40px 24px;
    gap: 30px;
  }

  .site-header span {
    font-size: 50px;
  }

  .main-img {
    width: 100%;
  }

  .bottom-row {
    width: 100%;
    flex-wrap: wrap;
    gap: 20px;
  }

  .bottom-row a {
    font-size: 18px;
  }

  .copy {
    font-size: 12px;
  }
}
</style>

<div class="page-wrap">

  <div class="site-header" onclick="showOverlay()">
    <span>JE'M</span>
  </div>

  <img class="main-img" src="{{ '/jem2.jpg' | relative_url }}">

  <div class="bottom-row">
    <a href="{{ '/lyrics' | relative_url }}">LYRICS</a>
    <a href="https://music.apple.com/jp/artist/jem/1864719862?l=en-US" target="_blank">APPLE MUSIC</a>
    <a href="https://www.youtube.com/@JEMMUSICJA" target="_blank">YOUTUBE</a>
    <div class="copy">© All rights reserved</div>
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
