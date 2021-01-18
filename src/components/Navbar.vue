<template>
  <ul class="Navbar">
      <template v-for="(page,index) in pages" :key="index">    
         <li v-if="page === 'Home'" class="Navbar-item active">
          {{page}}
         </li>
         <li  v-else class="Navbar-item">
          {{page}}
         </li>
      </template>        
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
    margin-left: 5%;
}

.Navbar-item{
    margin: 2em;
    color: white;
    font-family: 'Mazzard H',sans-serif;
    font-weight: 200;
    cursor: pointer;
    transition: 1s;
    font-size: .85em;
}

.Navbar-item.active, .Navbar-item:hover{
    font-family: 'Mazzard H',sans-serif;
    font-weight: bold;
    transform: scale(1.1,1.1);
}


@media screen and (max-width : 625px) {
    .Navbar{
        flex-direction: column;
       
    }

    .Navbar-item{
        width: 100%;
        justify-self: flex-start;
        margin: 1em;
    }
}

</style>