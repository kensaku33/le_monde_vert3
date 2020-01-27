<template>
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
</template>

<script>
$(function(){
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
  });   
})
</script>

<style>
/* 共通項目はSpring.vueに記載 */
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
  overflow: hidden;
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

</style>
