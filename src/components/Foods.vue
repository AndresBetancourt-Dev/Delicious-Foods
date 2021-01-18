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
                image : "../assets/bread.webp",
                title : "Bread"
            },
            {
                image : "../assets/burger.webp",
                title : "Hamburg"
            },
            {
                image : "../assets/cheese.webp",
                title : "Cheese"
            },
            {
                image : "../assets/meat.webp",
                title : "Meat"
            },
            {
                image : "../assets/donut.webp",
                title : "Doughnut"
            },
            {
                image : "../assets/ice-cream.webp",
                title : "ICE-Cream"
            },
            {
                image : "../assets/pizza.webp",
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
        margin: 0;
        padding: 0;
        list-style: none;
        justify-content: space-between;
    }
    .Food-container li{
        margin: 0;
        padding: 0;
    }

    @media screen and (max-width:750px) {
        .Food-container{
            flex-wrap: wrap;
        }
    }
</style>