<template>
  <div>我是其他页面
    <nuxt-link :to="{name:'users-class',params:{class:1001}}">我是测试页面</nuxt-link>
    <nuxt-link :to="{name:'users-id',params:{id:1002}}">我是详情页面</nuxt-link>
  </div>
</template>

<script>
export default{
  name: 'other'
}
</script>
