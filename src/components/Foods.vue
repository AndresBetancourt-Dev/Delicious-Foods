<template>
  <ul class="Food-container">
      <li  v-for="food in foods" :key="food.title">
          <Food :food="food"/>
      </li>
  </ul>
</template>

<script>
import Food from "./Food"
export default {
    setup(){
        const foods = [
            {
                image : "../assets/bread.png",
                title : "Bread"
            },
            {
                image : "../assets/burger.png",
                title : "Hamburg"
            },
            {
                image : "../assets/cheese.png",
                title : "Cheese"
            },
            {
                image : "../assets/meat.png",
                title : "Meat"
            },
            {
                image : "../assets/donut.png",
                title : "Doughnut"
            },
            {
                image : "../assets/ice-cream.png",
                title : "ICE-Cream"
            },
            {
                image : "../assets/pizza.png",
                title : "Pizza"
            }
        ]

        return {
            foods
        }
    },
    components : {
        Food,
    }
}
</script>

<style>
    .Food-container{
        width: 100vw;
        display: flex;
        height: auto;
        margin: 0;
        padding: 0;
        list-style: none;
        justify-content: space-between;
    }
    .Food-container li{
        margin: 0;
        padding: 0;
    }
</style>