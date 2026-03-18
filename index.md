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
  gap: 30px;
}

.site-header {
  margin-bottom: 10px;
}

.site-header a {
  font-size: 56px;
  text-decoration: none;
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

.right img {
  height: 55vh;
  width: auto;
  display: block;
}

.bottom {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  gap: 8px;
  width: fit-content;
  align-self: center;
  margin-left: calc(80px + /* leftの幅に合わせる */ 0px);
}

.bottom a {
  font-size: 28px;
  text-decoration: none;
  color: inherit;
}

.copy {
  font-size: 18px;
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
