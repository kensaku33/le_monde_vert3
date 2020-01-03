<template>
  <div class="header">
    <nav id="nav">
      <ul>

        <li class="mx-3">
          <router-link
            class="px-4"
            to="/"
            active-class="link--active"
            exact
            >
            home
          </router-link>
        </li>

        <li class="mx-3">
          <router-link 
            class="px-4" 
            to="/Order"
            active-class="link--active"
            exact
            >
            Order
          </router-link>
        </li>
        <li class="mx-3">contact</li>
        <li class="mx-3">what</li>
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
    background-color: #efeee8;
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
</style>