<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link>
      <router-link to="/about">About</router-link>
      <router-link to="/commission">Commissions</router-link>
    </div>

    <router-view id="view"/>

    <div class="spacer"></div>

  </div>
</template>

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
   justify-content: start !important;
   padding: $base-padding;
   box-shadow: 3px 0px 3px grey !important;
   min-height: 100%;

   
  a {
    margin-bottom: $base-margin;
  }
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
  justify-content: space-around;
  color: $darkpurple;
  background-color: $primary;
  box-shadow: 0px 2px 3px grey;

  a{
    color: whitesmoke;
    background-color: $primary;
  }
}



</style>
