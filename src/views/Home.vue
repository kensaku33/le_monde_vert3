<template>
  <div class="Home">
    <transition name="fade" appear>
      <div class="hello">
        <img src="@/assets/home-image.jpg" class="main-img img-fluid" alt="">
      </div>
    </transition>

    <div class="text">
      <h1 class="sample mb-5">sample message</h1>
      <p>たくしのこんなさびしい考は</p>
      <p>みんなよるのためにでるのだ</p>
      <p>夜があけて海岸へかかるなら</p>
      <p>そして波がきらきら光るなら</p>
      <p>なにもかもみんないいかもしれない</p>
    </div>



    <div class="sample mt-5">
      <h1 class="m-2">Parsonal color Sample</h1>
      <p class="your mb-5">あなたの色は？</p>
      <div class="sample-image mb-5">
          <!-- <div class="spring-box"></div> -->
          <img class="season-img img-fluid" src='https://lh3.googleusercontent.com/a1WiseEVAqwaXKrelUKmlxB_ZZd_EMRb0jvaPfIydzO3waMZBhcDXhkvytah8z84J9CvH1K6loWcmnf9osKhADoXuBabVVv6bJImd9NQr8RtwxVVfYsn46BCGzpN72CoKZrzUR0wyEM=w2400'>
          <div class="sample-image-text">spring</div>
      </div>

      <div class="sample-image mb-5">
          <img class="season-img img-fluid" src='https://lh3.googleusercontent.com/0Yw2epNLaQJqu_HG1A4MQ3NyOOHFuwsO8OPoP9U7QbuFuEMgax2NlgHY2H0G9MaTQ-xeHpYW7P1x-HUH55W7ZJsSotW56kR_gxOKGvalUfqsuHhE0aykBbb2_fhn-WHU6qTk2Eq17AU=w2400'>
          <div class="sample-image-text">summer</div>
      </div>

      <div class="sample-image mb-5">
          <img class="season-img img-fluid" src='https://lh3.googleusercontent.com/tS4W6LhL2Cs8ADylsD5TNW2iEOGEnYsbbaPJM-Ny-BQIBwwucCGpzAQ2HZI5OPl55d39G54S5me1IVIqOd1gEfEz_Sm3siMLLbAUZHCCVi8uG4APfDJcrzSrvb-EFMFNGdg9HAF-F6I=w2400' />
          <div class="sample-image-text">autumn</div>
      </div>

      <div class="sample-image mb-5">
          <img class="season-img img-fluid" src='https://lh3.googleusercontent.com/4W28sCXXNpYEEmb0N4m6wan38v0gmjJX9D0gnl3z0dTJddRKM1YTZM05Xz3wi5k1AQhS1gTnb68c5RbFD4H4QqCFdouTT9Zdi5sq7BwTr-OUC7K8GAl9ReXqBP0N0hS4v_-7zzRtwho=w2400' />
          <div class="sample-image-text">winter</div>
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

.your{
  font-size: 1.4rem;
}
.main-img{
  width:1200px;
  object-fit:cover;
}

.spring-box{
  background-color: green;
  height: 300px;
  width: 1200px;
}
.season-img{
  height: 300px;
  width: 1200px;
  object-fit: cover;
}
</style>