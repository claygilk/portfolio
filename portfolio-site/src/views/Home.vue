<template>
  <div class="home">
    <ul>
      <li v-for="link in links" :key="link">
        <img :src="link" alt="">
      </li>
    </ul>
    <!-- <img alt="Vue logo" src="https://i.ibb.co/cYwW3xW/kavaopaque.png"> -->
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import imageLinks from '@/assets/imageLinks.js'

export default {
  name: 'Home',
  components: {
    HelloWorld
  },
  data(){
    return{
      links: null,
    }
  },
  created(){
    this.links = imageLinks
  }
}
</script>

<style scoped>
img{
  width: 200px;
  height: auto;
}
</style>
