<template>
<div class="footer">
  <div class="footer-wrap">
    <div class="footer-left">
    <img src="@/assets/logo.png" class="footer-logo">
    </div>
    <div class="footer-info">
      <h4>LE MONDE VERT</h4>
      <hr>
        モンドベール
        <br>
        大阪府堺市南区宮山台2-3-1
        <br>
        info@monde-vert.com
    </div>
  </div>
  <br>
  <hr>
  <p class="copylight">
    ©︎ le monde vert
  </p>

</div>
</template>


<style scaped >

@media screen and (max-width: 640px) {
.footer{
  margin-top: 50vh;
  margin-bottom: 0;
  width: 100%;
  background-color:#efeee8;
  /* position: absolute;
  bottom: 0; */

}
.footer-wrap{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -ms-flex-pack:distribute;
  justify-content:space-around;
}
.footer-logo{
  height: 70px;
  margin: 60px 0 0 0px;
}
.footer-info{
  width: 100px;
  margin-top: 50px;
  text-align: right;
  float: right;
  font-size: 10px;
  /* background-color: yellow; */
}
.copylight{
  margin: 0;
  padding: 0 0 50px 0;
}
}

@media screen and (min-width: 640px) {
.footer{
  margin-top: 100px;
  width: 100%;
  background-color:#efeee8;
}
.footer-wrap{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -ms-flex-pack:distribute;
  justify-content:space-around;
}
.footer-logo{
  height:100px;
  margin: 60px 0 0 0px;
}
.footer-info{
  width: 220px;
  margin-top: 50px;
  text-align: right;
  float: right;
  /* background-color: yellow; */
}
.copylight{
  margin: 0;
  padding: 0 0 50px 0;
}
}
</style>