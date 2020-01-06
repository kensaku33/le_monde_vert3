<template>
  <div class="container">
    <div class="order-left-img"></div>
    <div class="order-right-contents col-auto">
      <h1 class="order-num">{{number}}</h1>
      <p class="order-text">{{text}}</p>
    </div>
  </div>
</template>

<script>
export default {
  data(){
    return{
      number: 'no.1',
      text: '目的、デザイン等の打ち合わせ',
    }
  }
}
</script>

<style scoped>
.container{
  position: relative;
  display: flex;
  margin: 200px 0;
}
.order-left-img{
  width: 500px;
  height: 500px;
  background-color: #efeee8d1;
}
.order-right-contents{
  position: absolute;
  left: 440px;
}
.order-num{
  font-size: 120px;
  color: #b9b9b9;
  text-align: left;
  border-bottom: 1px solid #b9b9b9;
}
.order-text{
  margin-top: 50px;
  color: #b9b9b9;
  text-align: left;
}
</style>