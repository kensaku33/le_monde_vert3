<template>
  <div class="header">
    <div class="logo">
      <router-link to="/">
        <img src="@/assets/logo.png" class="logo-img mt-4"/>
      </router-link>
    </div>
    <nav id="nav">
      <ul>
        <li class="mx-3">
          <router-link
            to="/"
            active-class="link--active"
            exact
            >
            home
          </router-link>
        </li>

        <li class="mx-3">
          <router-link 
            to="/Order"
            active-class="link--active"
            exact
            >
            order
          </router-link>
        </li>

        <li class="mx-3">
          <router-link 
            to="/Contact"
            active-class="link--active"
            exact
            >
            contact
          </router-link>
        </li>

        <li class="ml-1 mr-3">
          <b-nav-item-dropdown
            id="my-nav-dropdown"
            text="What"
            toggle-class="nav-link-custom"
            right
          >

          <b-dropdown-item>
            <a v-b-modal.modal-1>カラータイプ診断とは？</a>

              <b-modal id="modal-1" title="カラータイプ">
                <p class="my-4">Hello from modal!</p>
              </b-modal>

            </b-dropdown-item>


            <b-dropdown-item>
              <a v-b-modal.modal-2>ファッションタイプ？</a>
              <b-modal id="modal-2" title="ファッションタイプ">
                <p class="my-4">Hello from modal!</p>
              </b-modal>
            </b-dropdown-item>

            <b-dropdown-item>
              <a v-b-modal.modal-3>どんなオーダーが可能ですか？</a>
              <b-modal id="modal-3" title="こんなオーダーお待ちしています">
                <p class="my-4">Hello from modal!</p>
              </b-modal>
            </b-dropdown-item>
          </b-nav-item-dropdown>
        </li>

      </ul>
    </nav>
  </div>
</template>





<style>
  .header{
    position: absolute;
    top: 0;
    z-index: 3;
    height: 160px;
    width: 100%;
    background-color: #efeee8a9;
  }
  ul{
    position: absolute;
    right: 30px;
    bottom: 0;
  }
  li{
    display: inline-block;
    list-style: none;
  }

  .logo{
    margin: 0 auto;
    height:100px;
  }
  .logo-img{
    height: 100px;
  }

  @media screen and (max-width: 810px) {
    .header{
      position: absolute;
      top: 0;
      z-index: 3;
      height: 180px;
      width: 100%;
      background-color: #efeee8a9;
    }
  }

  @media screen and (max-width: 640px) {
    .header{
      position: absolute;
      top: 0;
      z-index: 3;
      height: 200px;
      width: 100%;
      background-color: #efeee8a9;
    }
  }
</style>