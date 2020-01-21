<template>
  <div class="Home">
    <transition name="fade" appear>
      <div class="hello">
        <img src="@/assets/home-image.jpg" class="main-img img-fluid" alt="">
      </div>
    </transition>

    <div class="text">
      <h1 class="sample mb-5">message</h1>
      <p>洋服は
        <br>
          色、形
        <br>
          そして素材から
        <br>
          成り立っています
        <br>
        <br>
          パーソナルカラーでお似合いの色を
        <br>
          ファッションテイスト診断で
        <br>
          引き立てるデザインと
        <br>
          素材をご提案します</p>
    </div>



    <div class="sample mt-5">
      <h1 class="m-2">Parsonal Color</h1>
      <p class="your mb-5">あなたの色は？</p>

    <!-- 春 -->
    <div class="season-wrapper">
      <div class="spring-box">
        <h2 class="season-title">spring</h2>
        <div class="season-btn" id="toggle-spring">show more</div>
      </div>
      <div class="spring-box-bottom">
        <div class="spring-inner-blur">
          <h2 class="spring-inner-title">spring</h2>
          <p class="spring-inner-text">
            スプリングタイプの人は、
            <br>
            <br>
            透明感のある健康的な肌、
            <br>
            ツヤのある髪、
            <br>
            <br>
            キラキラと輝くガラスのように
            <br>
            澄んだ瞳の持ち主。
            <br>
            <br>
            明るく華やかなタイプです。
          </p>
          <a class="show2" id="hide-spring">文字を隠す</a>
        </div>
      </div>
    </div>

    <!-- 夏 -->
    <div class="season-wrapper">
      <div class="summer-box">
        <h2 class="season-title">summer</h2>
        <div class="season-btn" id="toggle-summer">show more</div>
      </div>
      <div class="summer-box-bottom">
        <div class="summer-inner-blur">
          <h2 class="summer-inner-title">summer</h2>
          <p class="summer-inner-text">
            サマータイプの人は、
            <br>
            <br>
            きめ細やかなふわっとした肌、
            <br>
            やわらかくさらりとした髪、
            <br>
            <br>
            涼しげでソフトな瞳の持ち主。
            <br>
            <br>
            上品でしっとりとした
            <br>
            雰囲気を醸し出すタイプです。
          </p>
          <a class="show2" id="hide-summer">文字を隠す</a>
        </div>
      </div>
    </div>


    <!-- 秋 -->
    <div class="season-wrapper">
      <div class="autumn-box">
        <h2 class="season-title">autumn</h2>
        <div class="season-btn" id="toggle-autumn">show more</div>
      </div>
      <div class="autumn-box-bottom">
        <div class="autumn-inner-blur">
          <h2 class="autumn-inner-title">autumn</h2>
          <p class="autumn-inner-text">
            オータムタイプの人は、
            <br>
            <br>
            強い張りのあるつや肌、
            <br>
            ボリュームのあるナチュラルな髪、
            <br>
            <br>
            深みのある濃い瞳の持ち主。
            <br>
            <br>
            愛らしさと知性、
            <br>
            あたたかい雰囲気を漂わせています。
          </p>
          <a class="show2" id="hide-autumn">文字を隠す</a>
        </div>
      </div>
    </div>

    <!-- 冬 -->
    <div class="season-wrapper">
      <div class="winter-box">
        <h2 class="season-title">winter</h2>
        <div class="season-btn" id="toggle-winter">show more</div>
      </div>
      <div class="winter-box-bottom">
        <div class="winter-inner-blur">
          <h2 class="winter-inner-title">winter</h2>
          <p class="winter-inner-text">
            ウィンタータイプの人は、
            <br>
            <br>
            強く輝くシャープな瞳の持ち主。
            <br>
            <br>
            華やかな存在感が際立つタイプです。
            <br>
            <br>
            第一印象に残りやすいタイプです。
          </p>
          <a class="show2" id="hide-winter">文字を隠す</a>
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

// -------------------------------------------scroll-fadein---jquery
const obj = $(".season-wrapper")
$(window).on('scroll', function(){
  $(".season-wrapper").each(function(){
    const objPos = $(this).offset().top;
    const scroll = $(window).scrollTop();
    const windowH = $(window).height();
    if(scroll > objPos - windowH){
      $(this).css({
        'opacity': '1'
      });
    } else {
      $(this).css({
        'opacity': '0'
      });
    }
  });
});

// -------------------------------------------click-action---jquery

// --------------------------------------------spring

$(function(){
  var num1 = 0;
  $(document).on('click','#toggle-spring', function(){
    num1 = num1 + 1;
    
    if((num1 % 2)!= 0){
      $('.spring-box-bottom').css({
        height: '600px',
        opacity: '1',
      });
      $('.spring-inner-blur').css({
        width: '100%',
        transition: '1s',
      });
      $('.spring-inner-text, .spring-inner-title, #hide-spring').css({
        opacity: '1',
        transition: '2s',
      });
      $('#toggle-spring').text('close');
    }else{
      $('.spring-box-bottom').css({
        height: '0px',
        opacity: '0',
        transition: '1s',
      });
      $('.spring-inner-blur').css({
        width: '0%',
        transition: '1s',
      });
      $('.spring-inner-text, .spring-inner-title, #hide-spring').css({
        opacity: '0',
        transition: '1s',
      });
      $('#toggle-spring').text('show more');
    }
  });
  $(document).on('click','#hide-spring', function(){
    $('.spring-box-bottom').css({
      height: '800px',
      transition: '1s',
    });
    $('.spring-inner-blur').css({
      width: '0%',
      transition: '.8s',
    });
    $('.spring-inner-text, .spring-inner-title, #hide-spring').css({
      opacity: '0',
      transition: '.3s',
    });
  });   //-----------------------------------------spring

  // --------------------------------------------summer
  var num2 = 0;
  $(document).on('click','#toggle-summer', function(){
    num2 = num2 + 1;
    if((num2 % 2)!= 0){
      $('.summer-box-bottom').css({
        height: '600px',
        opacity: '1',
      });
      $('.summer-inner-blur').css({
        width: '100%',
        transition: '1s',
      });
      $('.summer-inner-text, .summer-inner-title, #hide-summer').css({
        opacity: '1',
        transition: '2s',
      });
      $('#toggle-summer').text('close');
    }else{
      $('.summer-box-bottom').css({
        height: '0px',
        opacity: '0',
        transition: '1s',
      });
      $('.summer-inner-blur').css({
        width: '0%',
        transition: '1s',
      });
      $('.summer-inner-text, .summer-inner-title, #hide-summer').css({
        opacity: '0',
        transition: '1s',
      });
      $('#toggle-summer').text('show more');
    }
  });
  $(document).on('click','#hide-summer', function(){
    $('.summer-box-bottom').css({
      height: '800px',
      transition: '1s',
    });
    $('.summer-inner-blur').css({
      width: '0%',
      transition: '.8s',
    });
    $('.summer-inner-text, .summer-inner-title, #hide-summer').css({
      opacity: '0',
      transition: '.3s',
    });
  });   //-----------------------------------------summer

  // --------------------------------------------autumn
  var num3 = 0;
  $(document).on('click','#toggle-autumn', function(){
    num3 = num3 + 1;
    if((num3 % 2)!= 0){
      $('.autumn-box-bottom').css({
        height: '600px',
        opacity: '1',
      });
      $('.autumn-inner-blur').css({
        width: '100%',
        transition: '1s',
      });
      $('.autumn-inner-text, .autumn-inner-title, #hide-autumn').css({
        opacity: '1',
        transition: '2s',
      });
      $('#toggle-autumn').text('close');
    }else{
      $('.autumn-box-bottom').css({
        height: '0px',
        opacity: '0',
        transition: '1s',
      });
      $('.autumn-inner-blur').css({
        width: '0%',
        transition: '1s',
      });
      $('.autumn-inner-text, .autumn-inner-title, #hide-autumn').css({
        opacity: '0',
        transition: '1s',
      });
      $('#toggle-autumn').text('show more');
    }
  });
  $(document).on('click','#hide-autumn', function(){
    $('.autumn-box-bottom').css({
      height: '800px',
      transition: '1s',
    });
    $('.autumn-inner-blur').css({
      width: '0%',
      transition: '.8s',
    });
    $('.autumn-inner-text, .autumn-inner-title, #hide-autumn').css({
      opacity: '0',
      transition: '.3s',
    });
  });   //-----------------------------------------autumn

  // --------------------------------------------winter
  var num4 = 0;
  $(document).on('click','#toggle-winter', function(){
    num4 = num4 + 1;
    if((num4 % 2)!= 0){
      $('.winter-box-bottom').css({
        height: '600px',
        opacity: '1',
      });
      $('.winter-inner-blur').css({
        width: '100%',
        transition: '1s',
      });
      $('.winter-inner-text, .winter-inner-title, #hide-winter').css({
        opacity: '1',
        transition: '2s',
      });
      $('#toggle-winter').text('close');
    }else{
      $('.winter-box-bottom').css({
        height: '0px',
        opacity: '0',
        transition: '1s',
      });
      $('.winter-inner-blur').css({
        width: '0%',
        transition: '1s',
      });
      $('.winter-inner-text, .winter-inner-title, #hide-winter').css({
        opacity: '0',
        transition: '1s',
      });
      $('#toggle-winter').text('show more');
    }
  });
  $(document).on('click','#hide-winter', function(){
    $('.winter-box-bottom').css({
      height: '800px',
      transition: '1s',
    });
    $('.winter-inner-blur').css({
      width: '0%',
      transition: '.8s',
    });
    $('.winter-inner-text, .winter-inner-title, #hide-winter').css({
      opacity: '0',
      transition: '.3s',
    });
  });   //-----------------------------------------winter
})

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
  margin-top: 100vh;
  margin-bottom: 200px;
  font-size: 18px;
}

.your{
  font-size: 1.4rem;
}
.main-img{
  position: absolute;
  top: 0;
  left: 0;
  width:100%;
  /* height: 100vh; */
  object-fit:cover;
}

/* 共通項 -----------------------共通項---------------------共通項------------------*/
.season-wrapper{
  font-size: 18px;
  margin: 400px 0;
  opacity: 0;
  transition: 2s;
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
  width: 0%;
  backdrop-filter: blur(10px);
}

.inner-title{
  color: white;
  font-size: 24px;
  padding-top: 100px;
  opacity: 0;
}
.inner-text{
  color: white;
  padding: 80px 0 50px 0;
  opacity: 0;
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
  transition: 1s;
  cursor: pointer;
  display: inline-block;
}
.show2:hover{
  letter-spacing: 5px;
  color: white;
}

/* 共通項 ------------------ ここまで ------------------- 共通項 ------------------- */


/* ------------------------------------------------------------spring */
.spring-box{
  width: 100%;
  height: 450px;
  background-color: #bcd094;
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
  height: 0px;
  opacity: 0;
  transition: 1s;
}
.spring-inner-blur{
  margin: 0 0 0 auto;
  height: 100%;
  width: 0%;
  backdrop-filter: blur(10px);
  /* padding: 50px; */
  background-color: #a0a0a030;
}

.spring-inner-title{
  color: white;
  font-size: 50px;
  padding-top: 60px;
  opacity: 0;
}
.spring-inner-text{
  color: white;
  padding: 60px 0 50px 0;
  opacity: 0;
}
#hide-spring{
  border: 1px solid white;
  color:white;
  padding: 10px 30px;

  transition: 1s;
  cursor: pointer;
  display: inline-block;
}
#hide-spring:hover{
  letter-spacing: 5px;
  color: white;
}


/* --------------------------------------------------------------ここまでspring */

/* ------------------------------------------------------------------summer  */

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
  height: 0px;
  transform: 1s;
  transition: 1s;
}
.summer-inner-blur{
  margin: 0 0 0 auto;
  height: 100%;
  width: 0%;
  backdrop-filter: blur(10px);
  background-color: #a0a0a030;
}

.summer-inner-title{
  color: white;
  font-size: 50px;
  padding-top: 60px;
  opacity: 0;
}
.summer-inner-text{
  color: white;
  padding: 60px 0 50px 0;
  opacity: 0;
}
#hide-summer{
  border: 1px solid white;
  color:white;
  padding: 10px 30px;

  transition: 1s;
  cursor: pointer;
  display: inline-block;
}
#hide-summer:hover{
  letter-spacing: 5px;
  color: white;
}

/* ----------------------------------------------------ここまでsummer */

/* ------------------------------------------------------autumn  */

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
  height: 0px;
  transform: 1s;
  transition: 1s;
}
.autumn-inner-blur{
  margin: 0 0 0 auto;
  height: 100%;
  width: 0%;
  backdrop-filter: blur(10px);
  background-color: #a0a0a030;
}

.autumn-inner-title{
  color: white;
  font-size: 50px;
  padding-top: 60px;
  opacity: 0;
}
.autumn-inner-text{
  color: white;
  padding: 60px 0 50px 0;
  opacity: 0;
}
#hide-autumn{
  border: 1px solid white;
  color:white;
  padding: 10px 30px;

  transition: 1s;
  cursor: pointer;
  display: inline-block;
}
#hide-autumn:hover{
  letter-spacing: 5px;
  color: white;
}

/* -------------------------------------------------------ここまでautumn */

/* -----------------------------------------------------------winter */

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
  height: 0px;
  transform: 1s;
  transition: 1s;
}

.winter-inner-blur{
  margin: 0 0 0 auto;
  height: 100%;
  width: 0%;
  backdrop-filter: blur(10px);
  background-color: #a0a0a030;
}
.winter-inner-title{
  color: white;
  font-size: 50px;
  padding-top: 60px;
  opacity: 0;
}
.winter-inner-text{
  color: white;
  padding: 60px 0 50px 0;
  opacity: 0;
}
#hide-winter{
  border: 1px solid white;
  color:white;
  padding: 10px 30px;

  transition: 1s;
  cursor: pointer;
  display: inline-block;
}
#hide-winter:hover{
  letter-spacing: 5px;
  color: white;
}

/* ---------------------------------------------------------ここまでwinter */


/* -------------------------------------------------------------mobile */
@media screen and (max-width: 640px) {
  .main-img{
    height:600px;
  }
  .spring-inner-title{
    color: white;
    font-size: 24px;
    padding-top: 60px;
    opacity: 0;
  }
  .spring-inner-text{
    color: white;
    padding: 60px 0 50px 0;
    opacity: 0;
  }

  .summer-inner-title{
    color: white;
    font-size: 24px;
    padding-top: 60px;
    opacity: 0;
  }
  .summer-inner-text{
    color: white;
    padding: 60px 0 50px 0;
    opacity: 0;
  }

  .autumn-inner-title{
    color: white;
    font-size: 24px;
    padding-top: 60px;
    opacity: 0;
  }
  .autumn-inner-text{
    color: white;
    padding: 60px 0 50px 0;
    opacity: 0;
  }

  .winter-inner-title{
    color: white;
    font-size: 24px;
    padding-top: 60px;
    opacity: 0;
  }
  .winter-inner-text{
    color: white;
    padding: 60px 0 50px 0;
    opacity: 0;
  }
}

.spring-box{
  width: 100%;
  height: 450px;
  background-color: #bcd094;
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
  height: 0px;
  opacity: 0;
  transition: 1s;
}
/* ---------------------------------------------------------------------- */

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