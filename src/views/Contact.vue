<template>
    <div>
        <transition name="fade" appear>
            <div class="hello">
                <img src="https://lh3.googleusercontent.com/VV780b0q1cAYToZe414q5zdGCPRECidz_YpNvLBs0tEC2q-ApfqQlT86g8wCsk4NuZ3MXf9HkQlYEXmczt5mjC_yYdJ3QCeAvC-YsoTgB917HlWuhygs37Q8b2vKB8K-mzNxVk8utEM=w2400" class="main-img img-fluid" alt="">
            </div>
        </transition>
            <div class="contact my-5">
                <h1 class="m-5">Contact</h1>
                <h1 class="address">LE MONDE VERT</h1>
                <h4>モンドベール</h4><br>
                <p class="address">大阪府堺市南区宮山台2-3-1</p>
                <p class="name">吉田加代 <br> Kayo Yoshida</p>
                <p class="mail">info@monde-vert.com</p>
            </div>
    </div>
</template>

<style scoped>
.hello{
    height: 120vh;
    width: 100vw;
    position: fixed;
    top: 50px;
    z-index: -3;
}
*{
    color: white;
}
@media screen and (max-width: 640px) {
    .main-img{
        height:600px;
        object-fit:cover;
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