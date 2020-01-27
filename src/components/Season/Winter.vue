<template>
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
</template>

<script>
$(function(){
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
  });
})
</script>

<style>
/* 共通項目はSpring.vueに記載 */

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
  overflow: hidden;
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
</style>