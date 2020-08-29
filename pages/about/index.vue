<template>
  <section id="about-page">
    <h1 class="aboutGreetColor">What About Me</h1>
      <div class="profile">
        <div class="myself">
          <h2 class="subPicColor">Profile</h2>
          <hr style="border-top: 1px dashed #cccccc;">
          <p>こんにちは。ひのいずと申します。プログラミング初学者です。日々プログラミング学習に奮闘中です。
                  Vue.jsとReact.jsが使って作成するのが好きです。</p>
          <p>I Want To Be A FrontEnd Developer!!</p>
        </div>
        <hr>
        <br>
        <div class="like">
          <h2 class="subPicColor">What I Like And Hobbies.</h2>
          <hr style="border-top: 1px dashed #cccccc;">
          <p>好きなことは映画を見ることが好きです。洋画の中でもコメディを好んで見ます。
                  話題の映画もよく見ます。家の中でも映画館で鑑賞するのも好きです。</p>
          <p>My Favorite Actors Are Adam Sandler, Seth Logen.</p>
        </div>
        <hr>
        <br>
        <div class="bgmy">
          <h2 class="subPicColor">Background</h2>
          <hr style="border-top: 1px dashed #cccccc;">
          <p>1996年: I Was Born!</p>
          <p>2015年: 京都の高校卒業</p>
          <p>2019年: 大阪の大学卒業</p>
          <p>2019年4月: 新卒で銀行入行。</p>
          <p>2019年10月: HTMLとCSSの学習スタート。人生初のコーディング。</p>
          <p>2019年11月: 学習に集中したいため退職。</p>
          <p>2020年2月: プログラミングの独学に限界を感じる。
            プログラミングスクール受講することを決意。
          </p>
          <p>2020年3月: Progate初挑戦。Rails Tutorialにも挑戦するも挫折。Ruby On Railsの環境構築も自身でやろうとするが、
            出来なかったため挫折。モチベーション下がる。
          </p>
          <p>2020年3月21日: スクールの受講日。本格的にプログラミング学習を始めたのはここからです。</p>
        </div>
        <hr>
        <br>
      </div>
  </section>
</template>

<style scoped>
#about-page {
  width: auto;
  height: auto;
  margin: 1rem;
  letter-spacing: 0.3rem;
  line-height: 2;
  font-family: "Noto Sans JP"; 
}


.aboutGreetColor {
  text-shadow:-5px 1px 6px rgba(17,240,228,0.92);
  animation-name: fadeIn;
  animation-duration: 3s;
  animation-timing-function: linear;
}

.subPicColor {
  text-shadow:-5px 1px 6px rgba(127,240,17,0.92);
  animation-name: fadeIn2;
  animation-duration: 3s;
  animation-timing-function: linear;
}

.profile {
 margin: 0 auto;
 width: 70vw;
  animation-name: fadeIn3;
  animation-duration: 2s;
  animation-timing-function: linear;
}

@keyframes fadeIn {
  from {
    opacity:0;
    text-shadow:-5px 1px 6px rgba(127,240,17,0.92);
  }
  to {
    opacity:1;
    text-shadow:-5px 1px 6px rgba(17,240,228,0.92);
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
</style>
