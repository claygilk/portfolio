<template>
  <div class="home">
    <img alt="Vue logo" src="https://i.ibb.co/cYwW3xW/kavaopaque.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld
  }
}
</script>
