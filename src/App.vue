<template>
  <div id="app">
      <Top id="top"></Top>
      <div class="nav-res">
        <div class="link-content-box">
          <a href="#" class="link-content" @click="clickSmoothScroll('#about')">
            <h3 class="comment">About</h3>
          </a>
        </div>
        |
        <div class="link-content-box">
          <a href="#" class="link-content" @click="clickSmoothScroll('#skills')">
            <h3 class="comment">Skills</h3>
          </a>
        </div>
        |
        <div class="link-content-box">
          <a href="#" class="link-content" @click="clickSmoothScroll('#works')">
            <h3 class="comment">Works</h3>
          </a>
        </div>
        |
        <div class="link-content-box">
          <a href="#" class="link-content" @click="clickSmoothScroll('#contact')">
            <h3 class="comment">Contact</h3>
          </a>
        </div>
        <div class="img-container">
          <img src='~@/assets/desk_img.png' width="70%">
        </div>
    </div>
      <div class="message">
        Nice to meet you. <br>
        My name is Gonshow Iqeda <br>
        who is learning engineering at UEC, in Japan. <br><br>

        Originality is a polished basis.<br>
        So, we should more cherish our groundwork.<br><br>

        I hope that the world will be fulled with grateful harvests.
      </div>
      <About id="about"></About>
      <Skills id="skills"></Skills>
      <Works id="works"></Works>
      <Contact id="contact"></Contact>
      <div class="tohome">
        <img src="./assets/home2.png" width="100" class="home">
        <a href="#" class="comment" @click="clickSmoothScroll('#top')">Home</a>
      </div>
      <Footer></Footer>
  </div>
</template>

<script>
import Top from './components/Top.vue'
import About from './components/About.vue'
import Skills from './components/Skills.vue'
import Works from './components/Works.vue'
import Contact from './components/Contact.vue'
import Footer from './components/Footer.vue'
export default {
  components: {
    Top,
    About,
    Skills,
    Works,
    Contact,
    Footer
  },
  methods:{
    clickSmoothScroll (x) {
      event.preventDefault()
      this.$SmoothScroll(
        document.querySelector(x),
        800,
        null,
        null,
        'y'
      )
    }
  }
}
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Comic+Neue:ital,wght@1,300&display=swap");

body {
background-image: url('./assets/body_background_img.jpg');
}
#app {
  font-family: 'Architects Daughter', cursive;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  //font-style: italic;
  font-weight: bold;
  font-size: 20px;
}

//メディアクエリで調整する
/*#skills {
  margin-right: 400px;
}*/


.res-title{
  //background-color: #98A51C;
  margin: 0;
  //background-color: whitesmoke;
  font-weight: bold;
}

.link-content-box {
  display: inline-block;
  width: 15%;
}
.comment {
  color:#2c3e50;
    -webkit-transition: all 0.5s ease-out;
    -moz-transition: all 0.5s ease-out;
    -ms-transition: all 0.5s ease-out;
    -o-transition: all 0.5s ease-out;
    transition: all 0.5s ease-out;
}
.comment:hover {
  color:#ff5500;
  -webkit-transform:rotateZ(5deg);
    -moz-transform:rotateZ(5deg);
    -ms-transform:rotateZ(5deg);
    -o-transform:rotateZ(5deg);
    transform:rotateZ(5deg);
    transform:rotateZ(-5deg);
}

.vue-typer .custom.char{
  color: aliceblue;
}
.content-title {
margin-top: 120px;
margin-bottom: 50px;
padding: 0.5em 0.5em;/*文字周りの余白*/
display: inline-block;/*おまじない*/
line-height: 1.3;/*行高*/
background-image: url('./assets/siori.png');
vertical-align: middle;
border-radius: 25px 0px 0px 25px;/*左側の角を丸く*/
box-shadow: 2px 0px 4px 0px gray
}
.content-title:before {
  content: '●';
  -webkit-background-clip: text;
  background-image: url('./assets/body_background_img.jpg');
  color: transparent;
  margin-right: 20px;
}
.message {
  padding: 20px;
}
a {
color:#2c3e50;
}
</style>
