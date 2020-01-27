<template>
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
</template>

<script>
$(function(){
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
  });
});
</script>

<style>
/* 共通項目はSpring.vueに記載 */
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
  overflow: hidden;
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

</style>