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
    width: 65%;
    height: auto;
    justify-content: space-between;
    align-items: center;
    position: relative;
    justify-self: center;
    align-self: center;
    padding: 0;
    margin: 0;
  }
  @media screen and (max-width: 950px) {
    .Header{
      flex-direction: column;
      margin-top: 2em;
    }
  }
</style>