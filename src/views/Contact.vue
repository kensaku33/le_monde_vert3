<template>
    <div>
        <transition name="fade" appear>
            <div class="contact-img">
                <img src="@/assets/Contact-img.jpg" class="main-img img-fluid" alt="">
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