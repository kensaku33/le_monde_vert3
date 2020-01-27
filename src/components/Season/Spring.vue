<template>
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
</template>

<script>

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
  });
});

</script>

<style>
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
  overflow: hidden;
}
.spring-inner-blur{
  margin: 0 0 0 auto;
  height: 100%;
  width: 0%;
  backdrop-filter: blur(10px);
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

</style>