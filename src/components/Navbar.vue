<template>
  <ul class="Navbar" v-for="(page,index) in pages" :key="index">     
     <div v-if="page === 'Home'">
         <li class="Navbar-item active">
          {{page}}
         </li>
     </div>
     <div v-else>
         <li class="Navbar-item">
          {{page}}
         </li>
     </div>
      
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
    font-family: 'Mazzard H',sans-serif;
    font-weight: 200;
}

.Navbar-item.active{
    font-family: 'Mazzard H',sans-serif;
    font-weight: bold;
}
</style>