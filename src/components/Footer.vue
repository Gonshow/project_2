<template>
  <div>
    <div class="footer">
      <h2>2020 ©️ Gonshow Iqeda</h2>
    </div>
  </div>
</template>
<style>
.block {
text-align: left;
margin-left: 5%;
}
.tohome {
  text-align: left;
}
.footer {
  border-top: rgba(12, 50, 78, 0.4) 3px solid;
    position: relative;
    margin-bottom: 40px;
    border-top: solid 1px #777777;
}
.footer:before, .footer:after{
    position: absolute;
    top: 0;
    content:'';
    width: 100%;
    height: 100%;
}
.footer:before{
    left:0;
    border-top: solid 1px #777777;
    transform: rotate(-0.5deg);
}
.footer:after{
    left:0;
    border-top: solid 1px #777777;
    transform: rotate(0.3deg);
}
</style>
