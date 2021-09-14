<template>
  <div id="main">
    <div class="links flex-row just-around">
        <div>
          <a href="https://www.instagram.com/morffaeus/">
            <i class="fab fa-instagram"></i> <span class="font-sm"> morffaeus </span>
          </a>
        </div>
        <div>
          <a href="https://discord.com/channels/@me" target="_blank">
            <i class="fab fa-discord"></i> <span class="font-sm"> Morffaeus #2866 </span> 
          </a>
        </div>
        <div id="email">
          <a href="mailto:nora.c.hinkle@gmail.com" >
            <i class="far fa-envelope"></i> <span class="font-sm">nora.c.hinkle@gmail.com</span> 
          </a>
        </div>
      </div>
  </div>
</template>

<script>
export default {
    name: "Footer"

}
</script>

<style lang="scss" scoped>

@import '../styles/index.scss';

@media only screen and (min-width: 720px) {
   .links{
       a{
           
           display: none !important;
       }
    } 
}

.links {


    a{
        display: block;
        color: $secondary;

    }
}


</style>