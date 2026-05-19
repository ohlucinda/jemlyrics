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

</style>

<div class="page-wrap">


<div class="bottom-row">
  <a href="{{ '/titles' | relative_url }}">LYRICS</a>

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
