<template>
  <div class="home">
    <div>
      <ul class="flex-row just-center">
        <li>
          <img src="@/assets/image0.png" alt="">
        </li>
        <li>
          <img src="@/assets/image1.png" alt="">
        </li>
        <li>
          <img src="@/assets/image4.png" alt="">
        </li>
        <li>
          <img src="@/assets/image2.png" alt="">
        </li>
        <li>
          <img src="@/assets/image3.png" alt="">
        </li>
      </ul>
    </div>
  </div>
</template>

<script>

export default {
  name: 'Home',
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
