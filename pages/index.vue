<template>
  <div class="nuxt-layout">
    <img src="@/assets/chizhiyiheng@240.png" alt="">
    <img src="/fenxiangxuetu@240.png" alt="">
    <nuxt-link to="/about">跳转about页面</nuxt-link>
  </div>
</template>

<script>
export default {
    name: "IndexPage",
}
</script>

<style scoped>
.nuxt-layout{
  background: url('~/assets/qiandao5@240.png') no-repeat;
  background-position-x: right;
}
</style>