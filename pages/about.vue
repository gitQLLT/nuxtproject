<template>
  <div class="jenies">
    我是about页面{{sex}}
    <nuxt-child />
    <nuxt-link to="/">跳转首页{{name}}</nuxt-link>
  </div>
</template>

<script>
export default {
  name: 'NuxtprojectAbout',
  transitions: 'about',
  middleware: 'static',
  data(){
    return{
      sex: '男'
    }
  },
  asyncData (context) {
    // called every time before loading the component
    return { name: 'World' }
  },
  fetch () {
    // The fetch method is used to fill the store before rendering the page
  },
  head () {
    // Set Meta Tags for this Page
  },
  mounted(){
    this.$myInjectedFunction('test')
  }
};
</script>

<style lang="scss" scoped>
.jenies{
  background: teal;
  a{
    color: red;
  }
}
</style>