<template>
  <div>
    <div v-if="error.statusCode == 404">
      404 页面不存在 {{error.message}}
    </div>
    <div v-else>
      应用程序错误
    </div>
    <nuxt-link to="/">首 页</nuxt-link>
  </div>
</template>

<script>
export default {
  props: ['error']
}
</script>

<style>

</style>
