<template>

<div class="order">
    <transition name="fade" appear>
        <div class="hello">
            <img src="@/assets/Order-img.jpg" class="main-img img-fluid" alt="">
        </div>
    </transition>
    <h2>Custom Order</h2>
    <p></p>

<!-- ---------------------------------------------------------container1 -->
<section>
    <div class="container ">
        <div class="order-left-img image1"></div>
        <div class="order-right-contents col-auto">
            <h1 class="order-num-odd">No.1</h1>
            <p class="order-text-odd">目的、デザインの打ち合わせ</p>
        </div>
        <div class="right-box"></div>
    </div>
</section>
<!-- ----------------------------------------------------------->
    
<!-- ---------------------------------------------------------container2 -->
<section>
    <div class="container">
        <div class="order-left-contents">
        <h1 class="order-num-even">No.2</h1>
        <p class="order-text-even">
            パーソナルカラーの診断
            <br>
            ファッションテイスト診断
            <br>
            <br>

            <span class="underbar">caution
                <br>
                ※料金が発生します
            </span>
            <br>
            </p>
        </div>
        <div class="order-right-img image2"></div>
    </div>
</section>
<!-- ----------------------------------------------------------->
    
<!-- ---------------------------------------------------------container3 -->
<section>
    <div class="container ">
        <div class="order-left-img image3"></div>
        <div class="order-right-contents col-auto">
        <h1 class="order-num-odd">No.3</h1>
        <p class="order-text-odd">デザイン、生地の提案</p>
        </div>
    </div>
</section>
<!-- ----------------------------------------------------------->
    
<!-- ---------------------------------------------------------container4 -->
<section>
    <div class="container ">
        <div class="order-left-contents">
        <h1 class="order-num-even">No.4</h1>
        <p class="order-text-even">
            型紙作成のための採寸
            </p>
        </div>
        <div class="order-right-img image4"></div>
    </div>
</section>
<!-- ----------------------------------------------------------->
    
<!-- ---------------------------------------------------------container5 -->

<section>
    <div class="container ">
        <div class="order-left-img image1"></div>
        <div class="order-right-contents col-auto">
        <h1 class="order-num-odd">No.5</h1>
        <p class="order-text-odd">目型紙作成
            <br>
            ジャケット、ワンピース
            <br>
            ¥40000-
            <br>
            パンツ、スカート、ブラウス
            <br>
            ￥20000-</p>
        </div>
    </div>
</section>

<!-- ----------------------------------------------------------->
    
<!-- ---------------------------------------------------------container6 -->
<section>
    <div class="container ">
        <div class="order-left-contents">
        <h1 class="order-num-even">No.6</h1>
        <p class="order-text-even">
            仮縫（かりぬい）
            </p>
        </div>
        <div class="order-right-img image4"></div>
    </div>
</section>
<!-- ----------------------------------------------------------->

<!-- ---------------------------------------------------------container7 -->

<section>
    <div class="container ">
        <div class="order-left-img image1"></div>
        <div class="order-right-contents col-auto">
        <h1 class="order-num-odd">No.7</h1>
        <p class="order-text-odd">生地決定、本縫い
※料金が発生します
	ジャケット、ワンピース　¥40000-
	パンツ、スカート、ブラウス　￥20000-</p>
        </div>
    </div>
</section>

<!-- ----------------------------------------------------------->

<!-- ---------------------------------------------------------container8 -->
<section>
    <div class="container ">
        <div class="order-left-contents">
        <h1 class="order-num-even">No.8</h1>
        <p class="order-text-even">
            試着、修正
            </p>
        </div>
        <div class="order-right-img image4"></div>
    </div>
</section>
<!-- ----------------------------------------------------------->

<!-- ---------------------------------------------------------container9 -->

<section>
    <div class="container ">
        <div class="order-left-img image1"></div>
        <div class="order-right-contents col-auto">
        <h1 class="order-num-odd">No.9</h1>
        <p class="order-text-odd">納品、請算（生地代、その他）</p>
        </div>
    </div>
</section>

<!-- ----------------------------------------------------------->

<div class="caution">
    <h3>▲Caution</h3>
    <p class="caution-text">
        ご確認ください
        <br>
        <br>
        ５、型紙作成時、７、本縫い時に料金が発生いたします。
        <br>
        ９、請算時は使用生地の代金の請算です。
        <br>
        <br>
        納期は進行過程により異なります。
        <br>
        仮縫などのご来店が必要なタイミングは納期に影響しますのでご注意ください。
    </p>
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

// -------------------------------------------scroll-fadein---jquery


$(window).on('scroll', function(){
    $(".container").each(function(){
        const objPos = $(this).offset().top;
        const scroll = $(window).scrollTop();
        const windowH = $(window).height();
        if(scroll > objPos - windowH){
            $(this).css({
                'opacity': '1'
            });
        } else {
            $(this).css({
                'opacity': '0'
            });
        }
    });

    // const leftIn = $(".order-left-img")
    // const rightText = $(".order-right-contents")
    // const rightIn = $(".order-right-img")
    // const leftText = $(".order-left-contents")

    


    // $(window).on('load resize', function(){
    //     var winW = $(window).width();
    //     var devW = 640;
    //     if (winW <= devW) {
    //         //----------------------------------------------640px以下の時の処理
    //         leftIn.each(function(){   // left-in
    //             const objPos = $(this).offset().top;
    //             const scroll = $(window).scrollTop();
    //             const windowH = $(window).height();
    //             if(scroll > objPos - windowH){
    //                 $(this).css({
    //                     'transform': 'translate(-100px,0)',
    //                     'transition': '1s'
    //                 })
    //             } else {
    //                 $(this).css({
    //                     'transform': 'translate(-200px,0)',
    //                     'transition': '1s'
    //                 });
    //             }
    //         });
    //         rightText.each(function(){   // left-in
    //             const objPos = $(this).offset().top;
    //             const scroll = $(window).scrollTop();
    //             const windowH = $(window).height();
    //             if(scroll > objPos - windowH){
    //                 $(this).css({
    //                     'transform': 'translate(0px,0)',
    //                     'transition': '1s',
    //                     opacity: '1'
    //                 })
    //             } else {
    //                 $(this).css({
    //                     'transform': 'translate(0px,100px)',
    //                     'transition': '1s',
    //                 opacity: '0'
    //                 })
    //             }
    //         });
    //         rightIn.each(function(){   // right-in
    //             const objPos = $(this).offset().top;
    //             const scroll = $(window).scrollTop();
    //             const windowH = $(window).height();
    //             if(scroll > objPos - windowH){
    //                 $(this).css({
    //                     'transform': 'translate(100px,0)',
    //                     'transition': '1s'
    //                 })
    //             } else {
    //                 $(this).css({
    //                     'transform': 'translate(200px,0)',
    //                     'transition': '1s'
    //                 });
    //             }
    //         });
    //         leftText.each(function(){
    //             const objPos = $(this).offset().top;
    //             const scroll = $(window).scrollTop();
    //             const windowH = $(window).height();
    //             if(scroll > objPos - windowH){
    //                 $(this).css({
    //                     'transform': 'translate(0px,0)',
    //                     'transition': '1s',
    //                     opacity: '1'
    //                 })
    //             } else {
    //                 $(this).css({
    //                     'transform': 'translate(0px,100px)',
    //                     'transition': '1s',
    //                 opacity: '0'
    //                 })
    //             }
    //         });
    //     } else {
    //         //----------------------------------------------640pxより大きい時の処理
    //         leftIn.each(function(){   // left-in
    //             const objPos = $(this).offset().top;
    //             const scroll = $(window).scrollTop();
    //             const windowH = $(window).height();
    //             if(scroll > objPos - windowH){
    //                 $(this).css({
    //                     'transform': 'translate(-100px,0)',
    //                     'transition': '1s'
    //                 })
    //             } else {
    //                 $(this).css({
    //                     'transform': 'translate(-200px,0)',
    //                     'transition': '1s'
    //                 });
    //             }
    //         });
    //         rightText.each(function(){   // left-in
    //             const objPos = $(this).offset().top;
    //             const scroll = $(window).scrollTop();
    //             const windowH = $(window).height();
    //             if(scroll > objPos - windowH){
    //                 $(this).css({
    //                     'transform': 'translate(0px,0)',
    //                     'transition': '1s',
    //                     opacity: '1'
    //                 })
    //             } else {
    //                 $(this).css({
    //                     'transform': 'translate(0px,100px)',
    //                     'transition': '1s',
    //                 opacity: '0'
    //                 })
    //             }
    //         });
    //         rightIn.each(function(){   // right-in
    //             const objPos = $(this).offset().top;
    //             const scroll = $(window).scrollTop();
    //             const windowH = $(window).height();
    //             if(scroll > objPos - windowH){
    //                 $(this).css({
    //                     'transform': 'translate(100px,0)',
    //                     'transition': '1s'
    //                 })
    //             } else {
    //                 $(this).css({
    //                     'transform': 'translate(200px,0)',
    //                     'transition': '1s'
    //                 });
    //             }
    //         });
    //         leftText.each(function(){
    //             const objPos = $(this).offset().top;
    //             const scroll = $(window).scrollTop();
    //             const windowH = $(window).height();
    //             if(scroll > objPos - windowH){
    //                 $(this).css({
    //                     'transform': 'translate(0px,0)',
    //                     'transition': '1s',
    //                     opacity: '1'
    //                 })
    //             } else {
    //                 $(this).css({
    //                     'transform': 'translate(0px,100px)',
    //                     'transition': '1s',
    //                 opacity: '0'
    //                 })
    //             }
    //         });
    //     }
    // });
// -------------------------------------------scroll-fadein---jquery-end
    const leftIn = $(".order-left-img")
    const rightText = $(".order-right-contents")
    leftIn.each(function(){   // left-in
        const objPos = $(this).offset().top;
        const scroll = $(window).scrollTop();
        const windowH = $(window).height();
        if(scroll > objPos - windowH){
            $(this).css({
                'transform': 'translate(-100px,0)',
                'transition': '1s'
            })
        } else {
            $(this).css({
                'transform': 'translate(-200px,0)',
                'transition': '1s'
            });
        }
    });
    rightText.each(function(){   // left-in
        const objPos = $(this).offset().top;
        const scroll = $(window).scrollTop();
        const windowH = $(window).height();
        if(scroll > objPos - windowH){
            $(this).css({
                'transform': 'translate(0px,0)',
                'transition': '1s',
                opacity: '1'
            })
        } else {
            $(this).css({
                'transform': 'translate(0px,100px)',
                'transition': '1s',
            opacity: '0'
            })
        }
    });



    const rightIn = $(".order-right-img")
    const leftText = $(".order-left-contents")
    rightIn.each(function(){   // right-in
        const objPos = $(this).offset().top;
        const scroll = $(window).scrollTop();
        const windowH = $(window).height();
        if(scroll > objPos - windowH){
            $(this).css({
                'transform': 'translate(100px,0)',
                'transition': '1s'
            })
        } else {
            $(this).css({
                'transform': 'translate(200px,0)',
                'transition': '1s'
            });
        }
    });
    leftText.each(function(){
        const objPos = $(this).offset().top;
        const scroll = $(window).scrollTop();
        const windowH = $(window).height();
        if(scroll > objPos - windowH){
            $(this).css({
                'transform': 'translate(0px,0)',
                'transition': '1s',
                opacity: '1'
            })
        } else {
            $(this).css({
                'transform': 'translate(0px,100px)',
                'transition': '1s',
            opacity: '0'
            })
        }
    });
});

</script>

<style scoped>
.container{
position: relative;
display: flex;
opacity: 0;
transition: 1.5s;
margin-bottom: 300px;
}

.one{
    opacity: 0;
}

.image1{
    background-image:url("https://lh3.googleusercontent.com/WSg0pT2Tc_7wH5A3wqWO3SzA5NTQRTJhlgGb_L9uGlZKuDqrhWquDZr9iGWNqbNpCtem6SgyGrLD5av0qbMQW62qIw3Osug3mWwn-qZbwSNHCDB0cxmi8rO5eF4iBZBBH5s6vcb4034=w2400");
}
.image2{
    background-image:url("https://lh3.googleusercontent.com/8lYJIYS5pD6G27Qurf53_wjYliXI52pk_9voMJSIHm8in9LC8LdzJqCjb_2ujTdptXFxDihRl3AljW4dGblGsS1t1L49f78_HWod9vEV5MW6Ye58sl4uKwjWtnA0Bm12Xrpzh9h6k4k=w2400");
}
.image3{
    background-image:url("https://lh3.googleusercontent.com/DyZN95Ehce2zgE2SrSFir2Fjo8gqhUlspfhhIpU6GXiOJHU72Trat8BfLju8ZALjRZd_VAXcvCo_jKZYP03VQm5YqkRip76MjYXFMrKFVAuuU0otv_DhfjBRBG2Mq-7Z_rT2vZ8DLXQ=w2400");
}
.image4{
    background-image:url("https://lh3.googleusercontent.com/Y_BtIupsprLVmAkR8Pvh4aKckD658OH3-u4SYkXaqPK4eeor257WyOUEyEg6ceP0GFzn3dhrrGM90ZBwF0kEWfO84WpcLyptlsFli1eLnUkuaSilwCEGFOeJIdM2eC2aDd7z1179SlA=w2400");
}
.image5{
    background-image:url();
}
.image6{
    background-image:url();
}
.image7{
    background-image:url();
}
.image8{
    background-image:url();
}
.image9{
    background-image:url();
}

.caution-text{
    white-space:pre;
}
/* -------------------------------------------------------odd contrents*/
.order-left-img{
width: 500px;
height: 500px;      
transform: translate(-200px,0);
background-repeat:  no-repeat;                         /* 画像の繰り返しを指定  */              
background-position:center center;                     /* 画像の表示位置を指定  */
background-size: cover;
}
.order-right-contents{
width: 300px;
transform: translate(0px,100px);
opacity: 0;
}
.order-num-odd{
font-size: 120px;
color: #b9b9b9;
text-align: left;
border-bottom: 1px solid #b9b9b9;
}
.order-text-odd{
margin-top: 50px;
color: #b9b9b9;
text-align: left;
}
.right-box{
    position: absolute;
    height: 200px;
    width: 300px;
    background-color: #efeee8d1;
    top: 200px;
    right: 0;
    z-index: -3;
}
/* ---------------------------------------------------------even contents*/
.underbar{
border-bottom: 1px solid #b9b9b9;
}
.order-left-contents{
position: absolute;
right: 520px;
width: 300px;
}
.order-num-even{
font-size: 120px;
color: #b9b9b9;
text-align: left;
border-bottom: 1px solid #b9b9b9;
}
.order-text-even{
margin-top: 50px;
color: #b9b9b9;
text-align: left;
}
.order-right-img{
margin: 0 0 0 auto;
width: 500px;
height: 500px;
background-color: #efeee8d1;
background-repeat:  no-repeat;  
background-position:center center;  
background-size: cover;
}

/* ------------------------------------------------------------------ */

/* -------------------------------------------------------------mobile */
@media screen and (max-width: 640px) {
    .container{
    position: relative;
    display: flex;
    opacity: 0;
    transition: 1.5s;
    margin-bottom: 300px;
    }
    .order-right-contents{
    top:700px;
    width: 300px;
    transform: translate(0px,100px);
    opacity: 0;
    }
    .order-num-odd{
    font-size: 120px;
    color: #b9b9b9;
    text-align: left;
    border-bottom: 1px solid #b9b9b9;
    }
    .order-text-odd{
    margin-top: 50px;
    color: #b9b9b9;
    text-align: left;
    }
}

/* --------------------------------------------------------------------- */
h2{
    color:#b9b9b9;
    font-size: 80px;
    margin: 200px 0;
}
h3{
    color:#b9b9b9;
    font-size: 50px;
    margin: 100px 0;
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