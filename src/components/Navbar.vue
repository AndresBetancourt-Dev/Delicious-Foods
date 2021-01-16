<template>
  <ul class="Navbar">
      <li v-for="(page,index) in pages" :key="index" class="Navbar-item">
          {{page}}
      </li>
  </ul>
</template>

<script>
export default {
    data(){
        return {
            pages : [
                "Home" , "Foods", "Success Stories", "About", "Sign up"
            ]
        }
    }
}
</script>

<style>
.Navbar{
    display: flex;
    text-decoration: none;
    list-style: none;
}

.Navbar-item{
    margin : 1em 3em;
    color: white;
}
</style>