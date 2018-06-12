<template>
  <div id="app">
    <ESportsCalendar msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
import ESportsCalendar from './components/ESportsCalendar.vue'

export default {
  name: 'app',
  components: {
    ESportsCalendar
  }
}
</script>

<style lang="scss">
$grid-breakpoints: (xs: 0, sm: 576px, md: 768px, lg: 992px, xl: 1200px) !default;
#app {
  font-family: 'Oswald', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #fff;
  height: 100%;
  background-image: linear-gradient(134deg, #424E75 0%, #262C4A 100%);;
}
body{
  margin: 0;
  height: 100%;
}
html{
  height: 100%;
}
</style>
