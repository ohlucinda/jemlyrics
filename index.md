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
  gap: 50px;
}

.site-header {
  cursor: pointer;
}

.site-header span {
  font-size: 70px;
  color: inherit;
}

.wrapper {
  display: flex;
  align-items: center;
  gap: 80px;
  flex: 1;
}

.left {
  display: flex;
  flex-direction: column;
  gap: 40px;
  flex-shrink: 0;
  align-self: center;
}

.left a {
  font-size: 50px;
  text-decoration: none;
  color: inherit;
}

.right-col {
  display: flex;
  flex-direction: column;
  gap: 12px;
}

.right-col img {
  width: 560px;
  height: auto;
  display: block;
}

.bottom {
  display: flex;
  flex-direction: column;
  align-items: flex-end;
  gap: 6px;
}

.bottom a {
  font-size: 24px;
  text-decoration: none;
  color: inherit;
  white-space: nowrap;
}

.copy {
  font-size: 16px;
  margin-top: 4px;
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

  .wrapper {
    flex-direction: column;
    gap: 30px;
    width: 100%;
  }

  .left {
    gap: 24px;
    width: 100%;
    align-self: auto;
  }

  .left a {
    font-size: 36px;
  }

  .right-col {
    width: 100%;
  }

  .right-col img {
    width: 100%;
    height: auto;
  }

  .bottom a {
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

  <div class="wrapper">
    <div class="left">
      <a href="{{ '/lyrics' | relative_url }}">LYRICS</a>
    </div>
    <div class="right-col">
      <img src="{{ '/jem2.jpg' | relative_url }}">
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
