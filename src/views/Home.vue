<template>
  <div class="Home">
    <transition name="fade" appear>
      <div class="hello">
        <img 
        src="https://lh3.googleusercontent.com/UlgVPV5wIbPNA6zLq3gGAHuhnO1o4xWS5jj919iEcrH68t77EKSBjUUL3E09suwB3ZBcEZlOMsX3GbXHk5ow3AjvtXTP1o7c_Q51PcoXN3uXBIu7L8AcaphtnTdtc0DsZMSlXJHnk8M=w2400" 
        class="main-img img-fluid" alt="">
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
      <p class="your my-5">which is your？</p>
      <Spring></Spring>
      <Summer></Summer>
      <Autumn></Autumn>
      <Winter></Winter>
    </div>
  </div>
</template>



<script>
import Spring from '@/components/Season/Spring.vue'
import Summer from '@/components/Season/Summer.vue'
import Autumn from '@/components/Season/Autumn.vue'
import Winter from '@/components/Season/Winter.vue'
export default {
  name: 'Home',
  data () {
    return {
      msg: 'おしゃれ心を呼び覚ます色彩の魅力、今までにないアプローチでお似合いのお洋服をご提案いたします。'
    }
  },
  components:{
    Spring,
    Summer,
    Autumn,
    Winter,
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
        'opacity': '1',
        transition: '.7s'
      });
    } else {
      $(this).css({
        'opacity': '0',
        transition: '.7s'
      });
    }
  });
});

</script>



<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.hello{
    height: 120vh;
    width: 100vw;
    position: fixed;
    top: 0;
    z-index: -3;
}

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
  color:white;
  margin-top: 100vh;
  margin-bottom: 200px;
  padding: 100px 0 200px 0;
  font-size: 18px;
  backdrop-filter: blur(10px);
  transition: .5s;
}
.text:hover{
  background-color: rgba(0, 0, 0, 0.112);
}

.your{
  color: white;
  font-size: 4rem;
}
.main-img{
  position: absolute;
  top: 0;
  left: 0;
  width:100%;
  /* height: 100vh; */
  object-fit:cover;
}


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