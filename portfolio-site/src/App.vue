<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link>
      <router-link to="/about">About</router-link>
      <router-link to="/commission">Commissions</router-link>
    </div>
    <router-view/>
  </div>
</template>

<style lang="scss">
#nav{
  display: flex;
  flex-flow: row wrap;
  justify-content: space-around;
}
</style>
