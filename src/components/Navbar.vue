<template>
  <ul>
      <li v-for="(page,index) in pages" :key="index">
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

</style>