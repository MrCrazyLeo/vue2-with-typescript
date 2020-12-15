<template>
  <div class="about">
    <h1>This is an about page</h1>
    <MyComponent />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import MyComponent from '@/views/Test.vue' // @ is an alias to /src

export default Vue.extend({
  name: 'Home',
  components: {
    MyComponent,
  },
})
</script>
