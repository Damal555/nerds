<template>
  <div id="app">
    <Slider/>
  </div>
</template>

<script>
import Slider from './components/Slider/Slider.vue'

export default {
  name: 'App',
  components: {
    Slider
  }
}
</script>

<style>
body{
  font-family: 'Roboto', 'Arial', sans-serif;
  font-weight: normal;
  font-size: 16px;
  line-height: 22px;
  font-weight: 500;
  color: #000;
}
</style>
