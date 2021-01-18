<template>
  <Hero/>
  <Foods/>
</template>

<script>
import Hero from "./components/Hero"
import Foods from "./components/Foods"
export default {
  components : {
    Hero,
    Foods
  }
  
}
</script>

<style>
@import url('./assets/fonts/Myriad/style.css');
@import url('./assets/fonts/Mazzard/stylesheet.css');
@import url('./assets/fonts/Morn/stylesheet.css');

*{
  box-sizing: border-box;
}

body{
  margin: 0;
  padding: 0;
  font-family: 'Myriad Pro Semibold',sans-serif;
  overflow-x: hidden;
}
</style>