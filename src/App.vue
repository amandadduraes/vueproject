<template>
  <div id="app" class="background-gradient">
    <MainMenu />
    <MainComponent />
    <router-view />
  </div>
</template>

<script>
import MainMenu from './components/MainMenu.vue';
import MainComponent from './components/MainComponent.vue';

export default {
  name: 'App',
  components: {
    MainMenu,
    MainComponent,
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
  background: linear-gradient(to bottom, #1b1b1b 50%, #f0f0f0 50%); 
}


</style>
