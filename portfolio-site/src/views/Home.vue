<template>
  <div class="home">
    <div>

      <ul class="flex-row just-center">
        <li id="test" :key="key" v-for="(img, key) in images">
       <img :src="img" class="" >
          
        </li>
      </ul>

    </div>
  </div>
</template>

<script>

export default {
  name: 'Home',
  data(){
    return {
      imageDir: '../assets',
      images: {}
    }
  },
  methods: {
    importAll(r) {
      var imgs = {}
      r.keys().forEach(key => (imgs[key] = r(key)))
      this.images = imgs
    }
  },
  mounted() {
    this.importAll(require.context('../assets', true, /\.png$/))
  },
}
</script>

<style lang="scss" scoped>
@import '@/styles/index.scss';

img{
  width: 350px;
  height: auto;
}

li{
  margin: $base-margin;
}

</style>
