<template>
 <div>
   <router-view /> <!--   把router组件显示在这里-->
   <hr />

 </div>
</template>

<style lang="scss">
@import "~@/assets/style/reset.scss";
@import "~@/assets/style/helper.scss";
body{
  line-height: 1.5;
  font-family: $font-hei;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  font-size: 16px;
  color: #333;
  background: #f5f5f5;
}

</style>