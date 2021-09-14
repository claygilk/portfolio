<template>
  <div id="app">
    <div id="nav">
      <div class="nav-links">
        <router-link to="/">Home</router-link>
        <router-link to="/contact">Contact</router-link>
        <router-link to="/commission">Commissions</router-link>
      </div>
      <div class="social-links ">
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

    <router-view id="view"/>

    <!-- <div class="spacer"></div> -->

    <Footer id="footer"/>

  </div>
</template>

<script>
import Footer from './components/Footer.vue'

export default {
  components: {
    Footer
  }
}
</script>

<style lang="scss">
@import './styles/index.scss';

// large screens
@media only screen and (min-width: 720px) {
 #app{
    display: flex;
    flex-direction: row;
    justify-content: space-between;
 }

 #nav {
   display: flex;
   flex-direction: column !important;
   align-items: center;
   justify-content: space-between !important;
   padding: $base-padding;
   box-shadow: 3px 0px 3px grey !important;
   min-height: 100%;

  a {
    margin-bottom: $base-margin;
  }
 }

 div.nav-links{
   display: flex;
   flex-direction: column !important;
   justify-content: space-between !important;
 }
 div.social-links{
   display: block !important;
 }
}

// small screens
#app{
  background-color: $secondary;
  min-height: 100vh;
  
}
#nav{
  display: flex;
  flex-flow: row wrap;
  justify-content: space-between;
  color: $darkpurple;
  background-color: $primary;
  box-shadow: 0px 2px 3px grey;

  a{
    color: whitesmoke;
    background-color: $primary;

  }
}

#email{
  white-space: nowrap;
}

div.nav-links{
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  width: 100%;
}

div.social-links{
  display: none;
}

#footer{
  position: fixed;
  bottom: 0;
  left: 0;
  right: 0;
  background-color: $darkpurple;
  color: white;
  
}

</style>
