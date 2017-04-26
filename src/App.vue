<template>
  <div id="app">
    <img src="./assets/logo.png">
    <vc-top-bar></vc-top-bar>
    <vc-main></vc-main>
    <vc-bottom-bar></vc-bottom-bar>
  </div>
</template>

<script>
import VcTopBar from './modules/layout/TopBar.vue'
import VcBottomBar from './modules/layout/BottomBar.vue'
import VcMain from './modules/users/Main.vue'

export default {
  
  name: 'app',
  components: {
    VcTopBar, VcBottomBar, VcMain
  },
  events: {
    'mudar-sentenca' (obj){
        windows.console.log(obj)
    }
  }
}
</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
