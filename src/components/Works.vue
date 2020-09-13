<template>
  <div>
    <h1 class="content-title">Works</h1>
    <ul class="works">
      <li class="blackboard">
        <img src='~@/assets/mas-img.gif' class="image" width="40%">
        <h2 class="work-title work1-title">MAS with Reinforcement Learning <a class="work-lang">(python)</a></h2>
        <p class="detail work1-detail">
          To model real world, I simulated encounted type diremma game using Multi Agent System.
        </p>
        <a href="https://github.com/Gonshow/MAS_sumilation" class="git-link work1-git-link" target="_blank">→ <a class="git-link-str">github</a></a>
      </li>
      <li class="blackboard">
        <img src='~@/assets/toeic-image.png' class="image work2-image" width="38%">
        <h2 class="work-title work2-title">Application to memorize English words for Toeic <a class="work-lang">(node.js, sqlite)</a></h2>
        <p class="detail work2-detail">
          You can learn English words by heart
          <br>to only choose correct one meaning
          <br>from three choices which is got out from SQL database.
        </p>
        <a href="https://github.com/Gonshow/quiz" class="git-link" target="_blank">→ <a class="git-link-str">github</a></a>
      </li>
      <li class="blackboard">
        <img src='~@/assets/work3-img.png' class="image work3-image" width="35%">
        <h2 class="work-title work3-title">Self made interpreter <a class="work-lang">(haskell)</a></h2>
        <p class="detail work3-detail">
          4 types of interpreters were created.
          <br>① Call by value, static scope
          <br>② Call by name, static scope
          <br>③ Call by value, dynamic scope
          <br>④ Continuation-passing style,
          <br>call by value, static scope
        </p>
        <a href="https://github.com/Gonshow/interpreter" class="git-link work3-git-link" target="_blank">→ <a class="git-link-str">github</a></a>
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
.blackboard {
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
.git-link:hover {
  opacity: 0.5;
}
.git-link-str {
  color: skyblue;
  border: groove 3px #D8CC41;
  border-radius: 50px 50px 40px 40px;/*左側の角を丸く*/
}
@media screen and (max-width: 480px) {
  .blackboard {
    display: inline-block;
    width: 250px;
    height: 185px;
    background-image: url('../assets/blackboard.png');
    background-size: cover;
    text-align: center;
    vertical-align: middle;
    margin: 0 auto;
    margin: 50px;
  }
 /*image, work-title, detail, git-linkをそれぞれについて調整*/
  /*以下default値*/
  .image {
    width: 35%;
    margin-top: 25px;
    margin-left: 15px;
    margin-right: 5px;
    float: left;
  }
  .work-title {
    font-size: 16px;
    margin-top: 25px;
  }
  .detail {
    font-size: 8px;
    margin-top: 17px;
  }
  .git-link {
    font-size: 10px;
    margin-bottom:0px;
  }
  /*以下で微調整*/
  .work2-image {
    width: 25%;
  }
  .work2-title {
    font-size: 13px;
  }
  .work2-detail {
    margin-top: 5px;
  }
  .work3-image {
    width: 28%;
  }
  .work3-title {
    font-size: 13px;
  }
  .work3-detail {
    margin-top: 0px;
  }
}
</style>
