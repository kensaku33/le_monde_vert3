<template>
  <div class="season-wrapper">
      <div class="autumn-box">
        <h2 class="season-title">autumn</h2>
        <div class="season-btn" id="toggle-autumn" v-on:click='toggle3=!toggle3'>show more</div>
      </div>
      <div class="autumn-box-bottom" v-bind:class='{verticalslide:toggle3}'>
        <div class="autumn-inner-blur" v-bind:class='{rightslide:toggle3}'>
          <h2 class="autumn-inner-title">autumn</h2>
          <p class="autumn-inner-text">
            オータムタイプの人は、
            <br>
            <br>
            強い張りのあるつや肌、
            <br>
            ボリュームのあるナチュラルな髪、
            <br>
            <br>
            深みのある濃い瞳の持ち主。
            <br>
            <br>
            愛らしさと知性、
            <br>
            あたたかい雰囲気を漂わせています。
          </p>
          <a class="show2" id="hide-autumn">文字を隠す</a>
        </div>
      </div>
    </div>
</template>
