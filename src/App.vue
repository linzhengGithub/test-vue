<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<style lang="scss">
  @import "~@/assets/style/helper.scss";
  @import "~@/assets/style/reset.scss";
  body{
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    font-family: $font-hei;
    line-height: 1.5;
    font-size: 16px;
    color: #333333;
    background: #f5f5f5;
  }
  @media (min-width: 500px) {
    #app{
      max-width: 500px;
      margin: 0 auto;
    }
  }
</style>
