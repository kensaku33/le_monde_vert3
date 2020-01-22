<template>

<div class="order">
    <transition name="fade" appear>
        <div class="hello">
            <img src="https://lh3.googleusercontent.com/yPoRXpyTSQW5h0_raL6f7lRgPO0JiIftaNbHYkS6qaUV4g8ludPwU1hAvao2RAKILMxfpCcYzrpHsjACrBf0rD7Ty8FC2A9N5Z0U-Zt9hdmWNiBizL2kmq4Df3DB6VeydjSp2pnDyWQ=w2400" class="main-img img-fluid" alt="">
        </div>
    </transition>
    <h2>Custom Order</h2>
    <p></p>

    <div id="short">工程の確認はこちら</div>

<!-- ---------------------------------------------------------container1 -->
<section>
    <div class="container background1">
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
    <div class="container background2">
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
    <div class="container background1">
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
    <div class="container background2">
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
    <div class="container background1">
        <div class="order-left-img image5"></div>
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
    <div class="container background2">
        <div class="order-left-contents">
        <h1 class="order-num-even">No.6</h1>
        <p class="order-text-even">
            仮縫（かりぬい）
            </p>
        </div>
        <div class="order-right-img image6"></div>
    </div>
</section>
<!-- ----------------------------------------------------------->

<!-- ---------------------------------------------------------container7 -->

<section>
    <div class="container background1">
        <div class="order-left-img image7"></div>
        <div class="order-right-contents col-auto">
        <h1 class="order-num-odd">No.7</h1>
        <p class="order-text-odd">
            生地決定、本縫い
            <br>
            ※料金が発生します
            <br>
            <br>
            ジャケット、ワンピース　¥40000-
            <br>
            パンツ、スカート、ブラウス　￥20000-</p>
        </div>
    </div>
</section>

<!-- ----------------------------------------------------------->

<!-- ---------------------------------------------------------container8 -->
<section>
    <div class="container background2">
        <div class="order-left-contents">
        <h1 class="order-num-even">No.8</h1>
        <p class="order-text-even">
            試着、修正
            </p>
        </div>
        <div class="order-right-img image8"></div>
    </div>
</section>
<!-- ----------------------------------------------------------->

<!-- ---------------------------------------------------------container9 -->

<section>
    <div class="container background1">
        <div class="order-left-img image9"></div>
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
        <span class="underbar">ご確認ください</span>
        <br>
        <br>
        ５、型紙作成時
        <br>
        ７、本縫い時に料金が発生いたします。
        <br>
        <br>
        ９、請算時は使用生地の代金の請算です。
        <br>
        <br>
        納期は進行過程により異なります。
        <br>
        仮縫などのご来店が必要なタイミングは
        <br>
        納期に影響しますのでご注意ください。
    </p>
</div>

<div class="modal-contents" id="modal">
    <div class="modal-inner">
    <p class="modal-inner-text">
        <span class="inner">オーダーの流れ</span>
        <br>
        <br>
        <br>

        <span class="line"></span>
        １、目的、デザイン等の打ち合わせ
        <br><br><br>
        ２、パーソナルカラーの診断
        <br>
        ファッションテイスト診断　
        <br>
        ＊料金が発生します　¥10000-
        <br><br><br>
        ３、デザイン、生地の提案
        <br><br><br>
        ４、型紙作成のための採寸
        <br><br><br>
        ５、型紙作成
        <br>
            　ジャケット、ワンピース
            <br>
            ¥40000-
            <br>
            　パンツ、スカート、ブラウス
            <br>
            ￥20000-
            <br><br><br>
        ６、仮縫
        <br><br><br>
        ７、生地決定、本縫い
        <br>
            　ジャケット、ワンピース
            <br>
            ¥40000-
            <br>
            　パンツ、スカート、ブラウス
            <br>
            ￥20000-
            <br>
            <br>
            <br>
        ８、試着、修正
        <br><br><br>
        ９、納品、請算（生地代、その他）
        <br><br><br>
        ＊ご注意
        <br><br>
        ５、型紙作成時、
        <br>
        ７、本縫い時に料金が発生いたします。
        <br>
        <br>
        ９、請算時は使用生地の代金の請算です。
        <br>
        <br>
        納期は進行過程により異なります。
        <br>
        <br>
        仮縫などのご来店が必要なタイミングは納期に影響しますのでご注意ください。
        </p>
    </div>
    <div class="close">close</div>
</div>


</div>

</template>










<script>


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
                'transition': '.6s',
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

    $(document).on('click','#short', function(){     //------modal
        $('#modal').fadeIn();
    });
    $(document).on('click','.close', function(){
        $('#modal').hide();
    })
});

</script>

<style scoped>
.hello{
    height: 120vh;
    width: 100vw;
    position: fixed;
    top: 0;
    z-index: -3;
}
.container{
position: relative;
display: flex;
opacity: 0;
transition: 1.5s;
margin-bottom: 300px;
padding: 0;
}

.background1{
    background-color: rgba(255, 255, 255, 0);
    backdrop-filter: blur(10px);
}
.background2{
    /* background-color: rgba(0, 0, 0, 0.263); */
    backdrop-filter: blur(10px);
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
    background-image:url("https://lh3.googleusercontent.com/28Dz_ZqoVdQjEeqTTEeoM16SXk_tROiCueuEodh9IXX2yPAyKW-o7yhR5XafsWO8MW3wcUZJDZBSh93vLr7udsW6LiEC3bQPjz_OZiwoqVayoZC-sYjZMYYUdLKk4q3NVklMdIxJ5wI=w2400");
}
.image6{
    background-image:url("https://lh3.googleusercontent.com/UlgVPV5wIbPNA6zLq3gGAHuhnO1o4xWS5jj919iEcrH68t77EKSBjUUL3E09suwB3ZBcEZlOMsX3GbXHk5ow3AjvtXTP1o7c_Q51PcoXN3uXBIu7L8AcaphtnTdtc0DsZMSlXJHnk8M=w2400");
}
.image7{
    background-image:url("https://lh3.googleusercontent.com/Zf_VQXz6OGluPiw55i3qH9iWnTV5n23Isro2Arymz7Ib57W_mNxv5nt_yhum71HSyUn-t31fQmjoyXk1qHpQw_tuKA7o02gdWV49ovtHNEUWXichfz246IME-J4w04G4SFDVFTZR-Bw=w2400");
}
.image8{
    background-image:url("https://lh3.googleusercontent.com/umb2ihY8iExeO8qUEktDQ5Rv79x77vKh-pZL6oEbq8nZZ3bAjUyUMBiMOWpzDPbEZ50Om6FmRgQ4Bc-dmNXccXicDZxtc3Qg4JmUdA7D6-NYy2OYoPiK7ATyEmY1FAxHZwJnWZ2XqN0=w2400");
}
.image9{
    background-image:url("https://lh3.googleusercontent.com/ovwT3y0LVR3Y1yFDw73QBNx0k5E7kt7QSGpfObF5n4Z4Z66v7-pUt7_zWhnikJuw6IJ_5B42MR_s_S7dPh9q4VfrbK7W-lxZR-Ra8CZqAocdTa2aRSaXmgotoCLLZQJYvwzdu4zaAQo=w2400");
}

.caution-text{
    white-space:pre;
}
/* -----------------------------------------------------------------------------------------------------------for PC */
@media screen and (min-width: 900px) {
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
    .order-left-img{/* -----------------------odd contrents*/
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
    color: #ffffff;
    text-align: left;
    border-bottom: 1px solid #ffffff;
    }
    .order-text-odd{
    margin-top: 50px;
    color: #ffffff;
    text-align: left;
    }
    /* ---------------------------------------------------------even contents*/
    .underbar{
    border-bottom: 1px solid #ffffff;
    }
    .order-left-contents{
    position: absolute;
    right: 520px;
    width: 300px;
    }
    .order-num-even{
    font-size: 120px;
    color: #ffffff;
    text-align: left;
    border-bottom: 1px solid #ffffff;
    }
    .order-text-even{
    margin-top: 50px;
    color: #ffffff;
    text-align: left;
    }
    .order-right-img{
    margin: 0 0 0 auto;
    width: 500px;
    height: 500px;
    background-repeat:  no-repeat;  
    background-position:center center;  
    background-size: cover;
    }
}


/* --------------------------------------------------------------------for tablet */
@media screen and (min-width: 640px) and (max-width:900px){
    .container{
        width: 60%;
        height: 700px;
        position: relative;
    }
    h2{
        color:#b9b9b9;
        font-size: 60px;
        margin: 200px 0;
    }
    h3{
        color:#b9b9b9;
        font-size: 50px;
        margin: 100px 0;
    }
    .order-left-img{/* -----------------------odd contrents*/
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
    position: absolute;
    top: 520px;
    left: 10px;
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
    /* ---------------------------------------------------------even contents*/
    .underbar{
    border-bottom: 1px solid #b9b9b9;
    }
    .order-left-contents{
    position: absolute;
    top: 520px;
    right: 0px;
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
}

/* -----------------------------------------------------------------------------------------------------------------------mobile */
@media screen and (max-width: 640px) {
    .main-img{
        height:550px;
        object-fit:cover;
    }

    .container{
        width: 100%;
        height: 700px;
        position: relative;
    }
    .order-left-img{
    min-width: 400px;
    height: 400px;      
    transform: translate(-200px,0);
    background-repeat:  no-repeat;                         /* 画像の繰り返しを指定  */              
    background-position:center center;                     /* 画像の表示位置を指定  */
    background-size: cover;
    }
    .order-right-contents{
    position: absolute;
    top: 440px;
    left: 10px;
    width: 300px;
    transform: translate(0px,100px);
    opacity: 0;
    }
    .order-num-odd{
    font-size: 60px;
    color: #b9b9b9;
    text-align: left;
    border-bottom: 1px solid #b9b9b9;
    }
    .order-text-odd{
    margin-top: 50px;
    color: #b9b9b9;
    text-align: left;
    }

    /* ---------------------------------------------------------even contents*/
    .underbar{
    border-bottom: 1px solid #b9b9b9;
    }
    .order-left-contents{
    position: absolute;
    top: 440px;
    left: 50px;
    width: 300px;
    }
    .order-num-even{
    font-size: 60px;
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
    width: 400px;
    height: 400px;
    background-color: #efeee8d1;
    background-repeat:  no-repeat;  
    background-position:center center;  
    background-size: cover; 
    }
    .caution-text{
        display: inline-block;
        
        height: 300px;
        width: 300px;
        font-size: 12px;
        color:#b9b9b9;
    }

    
}



/* --------------------------------------------------------------------- */

.caution-text{
        display: inline-block;
        height: 300px;
        width: 300px;
        font-size: 1rem;
        color:#ffffff;
    }
h2{
    color:#ffffff;
    font-size: 80px;
    margin: 200px 0;
}
h3{
    color:#ffffff;
    font-size: 50px;
    margin: 100px 0;
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

#short{
    border: 1px solid #b9b9b9;
    color: #b9b9b9;
    height: 50px;
    line-height: 50px;
    width: 200px;
    font-weight: 100;
    bottom: 50px;
    left: 0;
    right: 0;
    margin: 0 auto 300px auto;
    transition: .5s;
    cursor: pointer;
}
#short:hover{
    border: 1px solid white;
    color: white;
    background-color: #00000037;
}

.modal-contents{
    display: none;
    position: fixed;
    top: 0;
    left: 0;
    z-index: 100;
    width: 100vw;
    height: 100vh;
    background-color: rgba(0, 0, 0, 0.77);
    }
    .modal-inner{
    position:absolute;
    /* border: 1px solid white; */
    color: white;
    width: 50%;
    height: 65%;
    padding: 50px;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    margin: auto;
    background-color: rgba(0, 0, 0, 0.386);
    overflow: scroll;
    }
    .close{
    color: white;
    border: 1px solid white;
    text-decoration: none;
    text-shadow: none;
    height: 50px;
    line-height: 50px;
    width: 100px;
    font-weight: 100;
    position: absolute;
    bottom: 50px;
    right: 0px;
    left: 0;
    margin: auto;
    transition: .5s;
    opacity: 1;
    cursor: pointer;
    }
    .close:hover{
    color: white;
    opacity: .6;
    }
    .inner{
        font-size: 24px;
        padding: 0 0 3px 0;
        border-bottom: 1px solid white;
    }
</style>