<template>
  <div class="Home">
    <transition name="fade" appear>
      <div class="hello">
        <img src="@/assets/home-image.jpg" class="main-img img-fluid" alt="">
      </div>
    </transition>

    <div class="text">
      <h1 class="sample mb-5">message</h1>
      <p>洋服は、
        <br>
          色、形（デザイン）、素材から
        <br>
          成り立っています。
        <br>
        <br>
          パーソナルカラーでお似合いの色を、
        <br>
          ファッションテイスト診断で
        <br>
          引き立てるデザインと,
        <br>
          素材をご提案します</p>
    </div>



    <div class="sample mt-5">
      <h1 class="m-2">Parsonal color Sample</h1>
      <p class="your mb-5">あなたの色は？</p>

    <!-- 春 -->
    <div class="season-wrapper">
      <div class="spring-box">
        <h2 class="season-title">spring</h2>
        <div class="season-btn" id="down">show more</div>
      </div>
      <div class="spring-box-bottom">
        <div class="inner-blur">
          <h2 class="inner-title">春色の服</h2>
          <p class="inner-text">
            春はあけぼのちりぬるを
          <br>
          <br>
          夏は夕暮れ
          <br>
          <br>
          秋は紅葉が美しい
          </p>
          <a class="show2" id="hide">文字を隠す</a>
        </div>
      </div>
    </div>

    <!-- 夏 -->
    <div class="season-wrapper">
      <div class="summer-box">
        <h2 class="season-title">summer</h2>
        <div class="season-btn" id="down">show more</div>
      </div>
      <div class="summer-box-bottom">
        <div class="inner-blur">
          <h2 class="inner-title">夏色の服</h2>
          <p class="inner-text">
            春はあけぼのちりぬるを
          <br>
          <br>
          夏は夕暮れ
          <br>
          <br>
          秋は紅葉が美しい
          </p>
          <a class="show2" id="hide">文字を隠す</a>
        </div>
      </div>
    </div>


    <!-- 秋 -->
    <div class="season-wrapper">
      <div class="autumn-box">
        <h2 class="season-title">autumn</h2>
        <div class="season-btn" id="down">show more</div>
      </div>
      <div class="autumn-box-bottom">
        <div class="inner-blur">
          <h2 class="inner-title">秋色の服</h2>
          <p class="inner-text">
            春はあけぼのちりぬるを
          <br>
          <br>
          夏は夕暮れ
          <br>
          <br>
          秋は紅葉が美しい
          </p>
          <a class="show2" id="hide">文字を隠す</a>
        </div>
      </div>
    </div>

    <!-- 冬 -->
    <div class="season-wrapper">
      <div class="winter-box">
        <h2 class="season-title">winter</h2>
        <div class="season-btn" id="down">show more</div>
      </div>
      <div class="winter-box-bottom">
        <div class="inner-blur">
          <h2 class="inner-title">冬色の服</h2>
          <p class="inner-text">
            春はあけぼのちりぬるを
          <br>
          <br>
          夏は夕暮れ
          <br>
          <br>
          秋は紅葉が美しい
          </p>
          <a class="show2" id="hide">文字を隠す</a>
        </div>
      </div>
    </div>


    </div>

  </div>

</template>



<script>
export default {
  name: 'Home',
  data () {
    return {
      msg: 'おしゃれ心を呼び覚ます色彩の魅力、今までにないアプローチでお似合いのお洋服をご提案いたします。'
    }
  }
}
</script>



<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
.sample{
  margin-top: 100px;
  font-size: 50px;
}
.sample-image{
  position: relative;
}
.sample-image-text{
  position: absolute;
  font-size: 60px;
  top: 50%;
  left: 50%;
  -ms-transform: translate(-50%,-50%);
  -webkit-transform: translate(-50%,-50%);
  transform: translate(-50%,-50%);
  margin:0;
  padding:0;
}

.text{
  margin-bottom: 200px;
  font-size: 18px;
}

.your{
  font-size: 1.4rem;
}
.main-img{
  width:1200px;
  object-fit:cover;
}

/* 共通項 */
.season-wrapper{
  font-size: 18px;
  margin: 400px 0;
}
.season-title{
  font-size: 56px;
  padding-top: 100px;
}
.season-btn{
  border: 1px solid white;
  padding: 10px 30px;
  margin: 50px 30px;
  transition: 1s;
  font-size: 20px;
  cursor: pointer;
  display: inline-block;
}
.season-btn:hover{
  letter-spacing: 8px;
}


.inner-blur{
  margin: 0 0 0 auto;
  height: 100%;
  width: 50%;
  backdrop-filter: blur(10px);
}
.blur{
  animation-name: slideIn;
  animation-duration: 1s;
  animation-fill-mode: both;
  animation-delay: 1s;
}
@keyframes slideIn{
  0%{
    width:0%;
  }
  100%{
    width: 50%;
  }
}

.inner-title{
  color: white;
  font-size: 24px;
  padding-top: 100px;
}
.inner-text{
  color: white;
  padding: 80px 0 50px 0;

}
.show{
  border: 1px solid white;
  color:white;
  padding: 10px 30px;
  transition: 1s;
  cursor: pointer;
  display: inline-block;
}
.show:hover{
  letter-spacing: 14px;
}

.show2{
  border: 1px solid white;
  color:white;
  padding: 10px 30px;
  /* margin: 150px 30px; */
  transition: 1s;
  cursor: pointer;
  display: inline-block;
}
.show2:hover{
  letter-spacing: 5px;
  color: white;
}

.fade{
  animation-name: fadeIn;
  animation-duration: 1s;
  animation-fill-mode: both;
  animation-delay: 1.2s;
}
@keyframes fadeIn{
  0%{
    opacity: 0;
  }
  100%{
    opacity: 1;
  }
}
@-webkit-keyframes fadeIn{
    0% {
      opacity: 0;
      }
    100% {
      opacity: 1;
      }
}
/* ここまで */



.spring-box{
  width: 100%;
  height: 450px;
  background-color: #e8f3d2;
  color: white;
  text-align: center;
  padding: auto 0;
}
.spring-box-bottom{
  position: relative;
  background-repeat:  no-repeat;                         /* 画像の繰り返しを指定  */              
  background-position:center center;                     /* 画像の表示位置を指定  */
  background-size: cover;
  background-image:url("https://lh3.googleusercontent.com/a1WiseEVAqwaXKrelUKmlxB_ZZd_EMRb0jvaPfIydzO3waMZBhcDXhkvytah8z84J9CvH1K6loWcmnf9osKhADoXuBabVVv6bJImd9NQr8RtwxVVfYsn46BCGzpN72CoKZrzUR0wyEM=w2400");
  width: 100%;
  height: 600px;
  transform: 1s;
  transition: 1s;
}

.summer-box{
  width: 100%;
  height: 450px;
  background-color: #c4d0e8;
  color: white;
  text-align: center;
  padding: auto 0;
}
.summer-box-bottom{
  position: relative;
  background-repeat:  no-repeat;
  background-position:center center;
  background-size: cover;
  background-image: url("https://lh3.googleusercontent.com/0Yw2epNLaQJqu_HG1A4MQ3NyOOHFuwsO8OPoP9U7QbuFuEMgax2NlgHY2H0G9MaTQ-xeHpYW7P1x-HUH55W7ZJsSotW56kR_gxOKGvalUfqsuHhE0aykBbb2_fhn-WHU6qTk2Eq17AU=w2400");
  width: 100%;
  height: 600px;
  transform: 1s;
  transition: 1s;
}

.autumn-box{
  width: 100%;
  height: 450px;
  background-color: #e5c5b4;
  color: white;
  text-align: center;
  padding: auto 0;
}
.autumn-box-bottom{
  position: relative;
  background-repeat:  no-repeat;
  background-position:center center;
  background-size: cover;
  background-image: url("https://lh3.googleusercontent.com/tS4W6LhL2Cs8ADylsD5TNW2iEOGEnYsbbaPJM-Ny-BQIBwwucCGpzAQ2HZI5OPl55d39G54S5me1IVIqOd1gEfEz_Sm3siMLLbAUZHCCVi8uG4APfDJcrzSrvb-EFMFNGdg9HAF-F6I=w2400");
  width: 100%;
  height: 600px;
  transform: 1s;
  transition: 1s;
}

.winter-box{
  width: 100%;
  height: 450px;
  background-color: #c4dce8;
  color: white;
  text-align: center;
  padding: auto 0;
}
.winter-box-bottom{
  position: relative;
  background-repeat:  no-repeat;
  background-position:center center;
  background-size: cover;
  background-image: url("https://lh3.googleusercontent.com/4W28sCXXNpYEEmb0N4m6wan38v0gmjJX9D0gnl3z0dTJddRKM1YTZM05Xz3wi5k1AQhS1gTnb68c5RbFD4H4QqCFdouTT9Zdi5sq7BwTr-OUC7K8GAl9ReXqBP0N0hS4v_-7zzRtwho=w2400");
  width: 100%;
  height: 600px;
  transform: 1s;
  transition: 1s;
}




.season-img{
  height: 300px;
  width: 1200px;
  object-fit: cover;
}





.fade-enter{
    opacity: 0;
}
.fade-enter-active{
    transition: 2s;
}
.fade-enter-to{
    opacity: 1;
}
.fade-leave{
    opacity: 1;
}
.fade-leave-active{
    transition: 2s;
}
.fade-leave-to{
    opacity: 0;
}

</style>