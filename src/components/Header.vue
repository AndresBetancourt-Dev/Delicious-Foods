<template>
  <header class="Header">
      <Logo/>
      <Navbar/>
  </header>
</template>

<script>
import Navbar from "./Navbar"
import Logo from "./Logo"
export default {
    components : {
        Navbar,
        Logo
    }
}
</script>

<style>
  .Header{
    display: flex;
    width: 100%;
    height: auto;
    padding: 2em 7.5em 2em 17.5em;
    justify-content: space-between;
  }
</style>