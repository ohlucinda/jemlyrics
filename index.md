---
layout: default
---

<style>
body {
  font-size: 32px; /* ← 全体サイズを底上げ */
}

.wrapper {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 1100px;
  margin: 120px auto 60px; /* ← 上の余白しっかり */
}

.left {
  display: flex;
  flex-direction: column;
  gap: 40px; /* ← 行間バランス */
}

.name {
  font-size: 44px; /* ← Je'm をLYRICSと同じサイズに */
}

.lyrics {
  font-size: 44px;
}

.notes {
  font-size: 32px;
}

.right img {
  width: 420px;
}

.bottom {
  max-width: 1100px;
  margin: 40px auto;
  display: flex;
  flex-direction: column;
  align-items: flex-end;
  gap: 8px; /* ← 詰める */
}

.bottom a {
  font-size: 28px;
}

.copy {
  font-size: 18px;
  margin-top: 6px;
}

a {
  text-decoration: none;
  color: inherit;
}
</style>

<div class="wrapper">

  <div class="left">

    <a href="https://ohlucinda.wixsite.com/jemmusicja" target="_blank" class="name">
      MY NAME IS JE'M
    </a>

    <a href="{{ '/lyrics' | relative_url }}" class="lyrics">
      LYRICS
    </a>

    <a href="https://ohlucinda.wixsite.com/jemmusicja/blog" target="_blank" class="notes">
      MY NOTES
    </a>

  </div>

  <div class="right">
    <img src="{{ '/jem.jpg' | relative_url }}">
  </div>

</div>

<div class="bottom">

  <a href="https://music.apple.com/jp/artist/jem/1864719862?l=en-US" target="_blank">
    APPLE MUSIC
  </a>

  <a href="https://www.youtube.com/@JEMMUSICJA" target="_blank">
    YOUTUBE
  </a>

  <div class="copy">
    © All rights reserved
  </div>

</div>
