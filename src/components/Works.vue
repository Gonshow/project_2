<template>
  <div>
    <h1 class="content-title">Works</h1>
    <ul class="works">
      <li class="blackbord">
        <img src='~@/assets/mas-img.gif' class="image" width="40%">
        <h2 class="work-title">MAS with Reinforcement Learning <a class="work-lang">(python)</a></h2>
        <p class="detail">
          To model real world, I simulated encounted type diremma game using Multi Agent System.
        </p>
        <a href="https://github.com/Gonshow/MAS_sumilation" class="git-link" target="_blank">→ <a class="git-link-str">github</a></a>
      </li>
      <li class="blackbord">
        <img src='~@/assets/toeic-image.png' class="image" width="38%">
        <h2 class="work-title">Application to memorize English<br>words for Toeic <a class="work-lang">(node.js, sqlite)</a></h2>
        <p class="detail">
          You can learn English words by heart
          <br>to only choose correct one meaning
          <br>from three choices which is got out from SQL database.
        </p>
        <a href="https://github.com/Gonshow/quiz" class="git-link" target="_blank">→ <a class="git-link-str">github</a></a>
      </li>
      <li class="blackbord">
        <img src='~@/assets/work3-img.png' class="image" width="35%">
        <h2 class="work-title">Self made interpreter <a class="work-lang">(haskell)</a></h2>
        <p class="detail">
          4 types of interpreters were created.
          <br>① Call by value, static scope
          <br>② Call by name, static scope
          <br>③ Call by value, dynamic scope
          <br>④ Continuation-passing style,
          <br>call by value, static scope
        </p>
        <a href="https://github.com/Gonshow/interpreter" class="git-link" target="_blank">→ <a class="git-link-str">github</a></a>
      </li>
    </ul>
  </div>
</template>

<style>
.works{
  list-style-type: none;
  padding-left: 0;
  text-align: center;
}
.blackbord {
  display: inline-block;
  width: 500px;
  height: 500px;
  background-image: url('../assets/blackboard.png');
  background-size: 500px 500px;
  text-align: center;
  vertical-align: middle;
  margin: 0 auto;
  margin: 50px;
}
.image {
  margin-top: 50px;
  display: inline-block;
  transform: rotate(-1deg);
}
.work-title {
  transform: rotate(-3deg);
  color: white;
  padding-right: 10px;
}
.work-lang {
  color: #F7A291;
  margin: 0 0;
}
.detail {
  transform: rotate(-2deg);
  color: whitesmoke;
}
.git-link{
  text-decoration: none;
  color: skyblue;
  float: right;
  margin-right: 40px;
}
.git-link-str {
  color: skyblue;
  border: groove 3px #D8CC41;
  border-radius: 50px 50px 40px 40px;/*左側の角を丸く*/
}
</style>
