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
*{
  box-sizing: border-box;
}

body{
  margin: 0;
  padding: 0;
}
</style>