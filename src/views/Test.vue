<template>
  <button class="btn"
          @click="onClick">Click!</button>
</template>

<script lang="ts">
import Vue from 'vue'
// import Component from 'vue-class-component'
import Component from 'vue-class-component'

// Define the component in class-style
@Component
export default class MyComponent extends Vue {
  // 初始数据可以直接声明为实例的 property
  message = 'Hello！！'

  // 组件方法也可以直接声明为实例的方法
  onClick(): void {
    window.alert(this.message)
  }
}
</script>

<style scoped lang="less">
.btn {
  height: 40px;
  width: 100px;
  background-color: red;
}
</style>
