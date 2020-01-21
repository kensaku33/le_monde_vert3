<template>

  <div>
    <div class="header-top">
      <router-link to="/">
        <img src="@/assets/logo.png" class="logo-img mt-4"/>
      </router-link>
      <nav id="nav">
        <ul class="list">
          <li class="link">
            <router-link
              to="/"
              active-class="link--active"
              exact
              >
              home
            </router-link>
          </li>

          <li class="link">
            <router-link 
              to="/Order"
              active-class="link--active"
              exact
              >
              order
            </router-link>
          </li>

          <li class="link">
            <router-link 
              to="/Contact"
              active-class="link--active"
              exact
              >
              contact
            </router-link>
          </li>

          <li class="link" id="what">
            what
            <div class="what-box">
              <ul class="what-contents list-group">
                <li class="what-info" id="info1">
                  カラータイプ診断とは？
                </li>
                <li class="what-info" id="info2">
                  ファッションテイスト？
                </li>
                <li class="what-info" id="info3">
                  どんなオーダーが可能ですか？
                </li>
              </ul>
            </div>
          </li>
        </ul>
      </nav>

      <div id="menu">
        ▼　MENU　▼
      </div>
    </div>            <!-- header-top -->
    


    <div class="modal-contents" id="modal1">
      <div class="modal-inner">
        <p class="modal-inner-text">
          <span class="inner">
          カラータイプとは
          </span>
          <br>
          <br>
          その方の持つ　肌、目、髪の色を、
          <br>
          <br>
          どんな色がより引き立てるのかを示す理論です。
          <br>
          <br>
          「似合う」「似合わない」という個人の感覚だけでなく、
          <br>
          <br>
          法則、理論に基づいて診断していくため、パーソナルカラーを知ることで
          <br>
          <br>
          より自信を持っておしゃれを楽しむことができます</p>
        <div class="close">close</div>
      </div>
    </div>

    <div class="modal-contents" id="modal2">
      <div class="modal-inner">
        <p class="modal-inner-text">
          <span class="inner">
          ファッションテイストとは？
          </span>
          <br>
          <br>
          洋服のデザインと素材選びの方向性をどのようなイメージで統一するかを決める指標となるものです。
          <br>
          <br>
          当サロンでは、お客様の外見と内面の両方からみた診断と、
          <br>
          <br>
          パーソナルカラー診断で得られた情報も加味して、実際のサンプルを着用しながら
          <br>
          <br>
          ディテールの一つ一つを細かくチェックしていきます。
          </p>
        <div class="close">close</div>
      </div>
    </div>

    <div class="modal-contents" id="modal3">
      <div class="modal-inner">
        <p class="modal-inner-text">
          <span class="inner">
          こんな方がオーダーしています
          </span>
          <br>
          <br>
          ・自分にぴったりあった洋服を作りたい
          <br>
          <br>
          ・既製品だとどうしてもサイズが合わない
          <br>
          <br>
          ・お気に入りの服が古くなった。そっくりの服を作って欲しい
          <br>
          <br>
          ・生地があるのでそれで作って欲しい
        </p>
        <div class="close">close</div>
      </div>
    </div>
  </div>
</template>





<style scoped>
  .top{
    position: relative;
    top: 0;
    z-index: 3;
    height: 160px;
    width: 100%;
    background-color: #efeee8a9;
  }
  ul{
    right: 30px;
    bottom: 0;
  }
  li{
    display: inline-block;
    list-style: none;
  }
  #nav{
    height: 90px;
  }
  .header-top{
    margin: 0 auto;
    height:180px;
    position: relative;
    top: 0;
    z-index: 3;
    width: 100%;
    background-color: #efeee8a9;
  }
  .logo-img{
    height: 100px;
  }
  .list{
    position: absolute;
    margin-bottom: 0;
    right: 30px;
    bottom: 0px;
  }
  .link{
    height: 50px;
    line-height: 50px;
    margin-right: 30px;
  }
  #what{
    cursor: pointer;
  }
  #what:hover .whatbox{
    display: block;
  }
  .what-box{
    /* display: none; */
    position: absolute;
    right: 0px;
    padding-right: 0;
    margin-right: 0;
    top: 50px;
    z-index: 3;
  }
  .what-info{
    background-color: #efeee8a9;
    height: 50px;
    line-height: 50px;
    padding: 0 20px;
  }
  .what-info:hover{
    background-color: #efeee8de;
  }

  .modal-contents{
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
    left: 0;
    right: 0;
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
    font-size:1.5rem;
  }
  #menu{
    display: none;
  }

  @media screen and (max-width: 640px){/* ---------------------------------mobile */
    .header-top{
      margin: 0 auto;
      height:160px;
      position: relative;
      top: 0;
      z-index: 3;
      width: 100%;
      background-color: #efeee8;
    }

    li{
      margin: 0;
    }
    
    #menu{
      position: absolute;
      top: 120px;
      left: 0;
      right: 0;
      margin: auto;
      display: block;
      cursor: pointer;
    }

    .logo-img{
    height: 80px;
    }
    .list{
      display:none;
      position: absolute;
      top: 160px;
      left: 0;
      width: 100vw;
      padding: 0;
      margin: 0;

    }
    .link{
      width: 100vw;
      height: 50px;
      line-height: 50px;
      margin: 0px;
      background-color: #efeee8;
    }
    #what{
      cursor: pointer;
    }
    #what:hover .whatbox{
      display: block;
    }
    .what-box{
      /* display: none; */
      position: absolute;
      padding: 0;
      margin: 0;
      top: 200px;
      width: 100%;
      z-index: 3;
    }
    .what-info{
      background-color: #ffffff;
      height: 50px;
      line-height: 50px;
      padding: 0;
      margin: 0;
    }
    .what-info:hover{
      background-color: #efeee8;
    }


    .modal-inner{
      position:absolute;
      /* border: 1px solid white; */
      color: white;
      width: 80%;
      height: 85%;
      padding: 50px;
      top: 0;
      bottom: 0;
      left: 0;
      right: 0;
      margin: auto;
      background-color: rgba(0, 0, 0, 0.386);
    }
  }
</style>

<script>
$(function(){
  $('.what-contents').hide();
  $('.modal-contents').hide();

  $('#what').hover(function(){
    $('.what-contents:not(:animated)', this).slideToggle();
  });

  $(document).on('click','#info1', function(){     //------modal
    $('#modal1').fadeIn();
  });
  $(document).on('click', '#info2', function(){
    $('#modal2').fadeIn();
  });
  $(document).on('click','#info3', function(){
    $('#modal3').fadeIn();
  });

  $(document).on('click','.close', function(){
    $('#modal1, #modal2, #modal3').hide();
  })

  $('#menu').on('click', function(){
    $('.list').toggle();
  })

});
</script>