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
button {
  font-family: 'Oswald', sans-serif;
}
body{
  margin: 0;
  height: 100%;
}
html{
  height: 100%;
}
.margins-grid {
  margin-left: 10%;
  margin-right: 10%;
}
.font-size-l {
  font-size: 28px;
  line-height: 35px;
  margin: 0;
   @media (min-width: map-get($grid-breakpoints, sm)){
     font-size: 18px;
    line-height: 22px;
   }
   @media (min-width: map-get($grid-breakpoints, md)){
     font-size: 24px;
    line-height: 28px;
   }
}
.font-size-xl {
  font-size: 35px;
  line-height: 35px;
  margin: 0;
   @media (min-width: map-get($grid-breakpoints, sm)){
     font-size: 40px;
    line-height: 45px;
   }
   @media (min-width: map-get($grid-breakpoints, md)){
     font-size: 60px;
    line-height: 65px;
   }
}
.uppercase {
  text-transform: uppercase;
}
.font-weight-sb {
  font-weight: 600;
}
</style>
