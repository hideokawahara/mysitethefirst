<template> 
  <section id="works-page"> 
      <h1 class="greet">Thank You For Comming.</h1>
      <div class="contents">
        <h2 style="text-align: center;">Web Developer</h2>
        <br>
        <hr>
        <h2 class="subtitle">What I Have Ever Used.</h2>
        <div class="skills">
          <div class="skill frontend">
            <h2 class="frontend-title">FrontEnd</h2>
            <div style="font-family: 'Poppins', sans-serif; font-weight: 700; text-align: center;">
              <p class="block">JavaScript</p>
              <p class="block">Vue.Js</p>
              <p class="block">React.js</p>
            </div>
          </div>
          <div class="skill backend">
            <h2 class="backend-title">BackEnd</h2>
            <div style="font-family: 'Poppins', sans-serif; font-weight: 700; text-align: center;">
              <p class="block">Ruby</p>
              <P class="block">Node.Js</P>
            </div>
          </div>
        </div>
      </div>
  </section> 
</template>

<style scoped>
#works-page {
  width: auto;
  /* height: auto; */
  margin: 1rem;
  letter-spacing: 0.3rem;
  line-height: 2;
  font-family: "Noto Sans JP"; 
  /* height: 100vh; */
  
}

.greet {
  text-shadow:-5px 1px 6px rgba(127,240,17,0.92);
  animation-name: fadeIn2;
  animation-duration: 3s;
  animation-timing-function: linear;
}

.contents {
  margin: 0 auto;
  width: 70vw;
  animation-name: fadeIn3;
  animation-duration: 2s;
  animation-timing-function: linear;
}

.subtitle {
  font-size: 2.5rem; 
  display: inline-block;
  text-shadow:36px -8px 3px #ca00fa;
  animation-name: moveFont;
  animation-duration: 3s;
  animation-timing-function: linear;
}

.skills {
  display: flex;
  justify-content: center;
  flex-direction: column;
} 

.skill {
  margin: 3rem 3rem 5rem;
  text-align: center;
}

.frontend-title {
  /* background-color: #65a6d4; */
  background:
      linear-gradient(217deg, rgba(0,0,255,.8), rgba(255,0,0,0) 70.71%),
      linear-gradient(127deg, rgba(0,255,0,.8), rgba(0,255,0,0) 70.71%),
      linear-gradient(336deg, white, rgba(0,0,255,0) 70.71%);
  border-radius: 100px;
  color: white;
  padding: 0 2rem;
  display: inline-block;
}

.backend-title {
  /* background-color: #d66d8c; */
  background:
      linear-gradient(217deg, rgba(0,255,0,.8), rgba(255,0,0,0) 70.71%),
      linear-gradient(127deg, rgba(0,0,255,.8), rgba(0,255,0,0) 70.71%),
      linear-gradient(336deg, white, rgba(0,0,255,0) 70.71%);
  border-radius: 100px;
  color: white;
  padding: 0 2rem;
  display: inline-block;
}

.block {
  display: flex;
  flex-direction: column; 
  /* display: inline-block; */
  /* flex-direction: column; */
  margin-left: auto;
  margin-right: auto;
}

@media (min-width: 35rem) {
  .skills {
    flex-direction: row;
    /* flex-wrap: wrap; */
  }

  .frontend-title,
  .backend-title {
    padding: 0 2rem;
    display: inline-block;
  }
}

@keyframes fadeIn2 {
  from {
    opacity:0;
    text-shadow:-5px 1px 6px rgba(17,240,228,0.92);
  }
  to {
    opacity:1;
    text-shadow:-5px 1px 6px rgba(127,240,17,0.92);
  }
}

@keyframes fadeIn3 {
  from {
    opacity:0;
  }
  to {
    opacity:1;
  }
}

@keyframes moveFont {
  from {
    opacity:0;
    font-size: 2rem; 
    display: inline-block;
    text-shadow:2px 28px 3px #fa0068;
  }
  to {
    opacity:1;
    font-size: 2.5rem; 
    display: inline-block;
    text-shadow:36px -8px 3px #ca00fa;
  }
}
</style>
