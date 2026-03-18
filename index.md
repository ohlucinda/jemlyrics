---
layout: default
---

<style>
.page-wrap {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  box-sizing: border-box;
  font-family: 'Aboreto', cursive;
}

.site-header {
  text-align: center;
  font-size: 44px;
  padding: 30px 0;
}

.site-header a {
  text-decoration: none;
  color: inherit;
}

.wrapper {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex: 1;
  padding: 0 60px;
  gap: 40px;
}

.left {
  display: flex;
  flex-direction: column;
  gap: 40px;
}

.left a {
  font-size: 44px;
  text-decoration: none;
  color: inherit;
  white-space: nowrap;
}

.right {
  flex: 1;
  max-width: 50%;
  display: flex;
  justify-content: flex-end;
}

.right img {
  width: 100%;
  max-height: 70vh;
  object-fit: cover;
  display: block;
}

.bottom {
  display: flex;
  flex-direction: column;
  align-items: flex-end;
  gap: 8px;
  padding: 30px 60px;
}

.bottom a {
  font-size: 23px;
  text-decoration: none;
  color: inherit;
}

.copy {
  font-size: 16px;
  margin-top: 6px;
}
</style>

<div class="page-wrap">

  <div class="site-header">
    <a href="{{ '/' | relative_url }}">JE'M</a>
  </div>

  <div class="wrapper">

    <div class="left">
      <a href="https://ohlucinda.wixsite.com/jemmusicja" target="_blank">MY NAME IS JE'M</a>
      <a href="{{ '/lyrics' | relative_url }}">LYRICS</a>
      <a href="https://ohlucinda.wixsite.com/jemmusicja/blog" target="_blank">MY NOTES</a>
    </div>

    <div class="right">
      <img src="{{ '/jem.jpg' | relative_url }}">
    </div>

  </div>

  <div class="bottom">
    <a href="https://music.apple.com/jp/artist/jem/1864719862?l=en-US" target="_blank">APPLE MUSIC</a>
    <a href="https://www.youtube.com/@JEMMUSICJA" target="_blank">YOUTUBE</a>
    <div class="copy">© All rights reserved</div>
  </div>

</div>
