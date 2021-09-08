<template>
  <div class="home">
    <div>
      <ul>
        <li>
          <img src="@/assets/image0.png" alt="">
        </li>
        <li>
          <img src="@/assets/image1.png" alt="">
        </li>
        <li>
          <img src="@/assets/image2.png" alt="">
        </li>
        <li>
          <img src="@/assets/image3.png" alt="">
        </li>
        <li>
          <img src="@/assets/image4.png" alt="">
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import imageLinks from '@/assets/imageLinks.js'

export default {
  name: 'Home',
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
