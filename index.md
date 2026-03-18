---
layout: default
---

<style>
body {
  margin: 0;
}

/* 全体レイアウト */
.wrapper {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 1100px;
  margin: 120px auto 60px;
}

/* 左（メインリンク） */
.left {
  display: flex;
  flex-direction: column;
  gap: 40px;
}

/* 上3つ：完全に同じサイズ */
.left a {
  font-size: 44px;
  text-decoration: none;
  color: inherit;
}

/* 右画像 */
.right img {
  width: 420px;
}

/* 下（外部リンク） */
.bottom {
  max-width: 1100px;
  margin: 40px auto;
  display: flex;
  flex-direction: column;
  align-items: flex-end;
  gap: 8px;
}

/* 下リンクは元のサイズ維持 */
.bottom a {
  font-size: 23px;
  text-decoration: none;
  color: inherit;
}

/* コピー */
.copy {
  font-size: 16px;
  margin-top: 6px;
}
</style>

<div class="wrapper">

  <div class="left">

    <a href="https://ohlucinda.wixsite.com/jemmusicja" target="_blank">
      MY NAME IS JE'M
    </a>

    <a href="{{ '/lyrics' | relative_url }}">
      LYRICS
    </a>

    <a href="https://ohlucinda.wixsite.com/jemmusicja/blog" target="_blank">
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
