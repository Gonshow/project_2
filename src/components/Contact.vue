<template>
  <div class="contacts">
    <h1 class="content-title">Contact</h1>
    <div class="contact-container">
      <h2> Click !!</h2>
      <div class="link">
        <a href="https://www.instagram.com/kunnerzhigh/" class="link-icon" target="_blank"><img src='~@/assets/insta.png' width="70"></a>
        <a href="https://www.facebook.com/exit.ajisai/" class="link-icon" target="_blank"><img src='~@/assets/facebook.png' width="70"></a>
        <a href="https://github.com/Gonshow" class="link-icon" target="_blank"><img src='~@/assets/github-icon.svg' width="70"></a>
        <a href="mailto:i2030012@uec.cc.uec.ac.jp" class="link-icon"><img src='~@/assets/mail.png' width="70"></a>
      </div>
    </div>
  </div>
</template>
<style>
.link-icon img{
  margin: 10px;
  -webkit-transition: all 0.5s ease-out;
  -moz-transition: all 0.5s ease-out;
  -ms-transition: all 0.5s ease-out;
  -o-transition: all 0.5s ease-out;
  transition: all 0.5s ease-out;
}
.link-icon:hover img{
  -webkit-transform:rotateZ(15deg);
    -moz-transform:rotateZ(15deg);
    -ms-transform:rotateZ(15deg);
    -o-transform:rotateZ(15deg);
    transform:rotateZ(-25deg);
}
</style>
