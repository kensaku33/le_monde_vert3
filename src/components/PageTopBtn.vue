<template>
  <div id="page-top" v-on:click="moveToTop">
    ▲
  </div>
</template>

<script>
export default {
  methods:{
    moveToTop(){
      const duration = 1000;
      const interval = 25;
      const step = -window.scrollY / Math.ceil(duration / interval);
      const timer = setInterval(() => {
        window.scrollBy(0,step);
        if(window.scrollY <= 0){
          clearInterval(timer);
        }
      }, interval);
    }
  }
}
</script>

<style scaped>
  #page-top{
    height: 60px;
    width: 60px;
    border-radius: 50%;
    background-color: #7070700d;
    position: fixed;
    z-index: 10;
    right: 100px;
    top: 500px;
    transition: .5s;
    color: rgba(255, 255, 255, 1.0);
    line-height: 60px;
  }
  #page-top:hover{
    transition: .5s;
        background-color: #707070;
  }

  #arrow{
    font-size: 2rem;
    padding-top: 20px;
  }
</style>