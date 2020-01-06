<template>

<div class="order">
    <transition name="fade" appear>
        <div class="hello">
            <img src="@/assets/Order-img.jpg" class="main-img img-fluid" alt="">
        </div>
    </transition>
    <h2>Custom Order</h2>
    <p></p>
    <Order1></Order1>
    <Order2></Order2>
    <Order3></Order3>
    <Order4></Order4>
    <Order5></Order5>
</div>

</template>

<script>
import Order1 from '../components/Order/Order1.vue'
import Order2 from '../components/Order/Order2.vue'
import Order3 from '../components/Order/Order3.vue'
import Order4 from '../components/Order/Order4.vue'
import Order5 from '../components/Order/Order5.vue'
export default {
    components:{
        Order1,
        Order2,
        Order3,
        Order4,
        Order5,
    }
}
</script>

<style scoped>
h2{
    color:#b9b9b9;
    font-size: 80px;
    margin: 200px 0;
}
.background{
    width: 100%;
    height: 400px;
    background-color: aquamarine;
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