<template>
    <div class="Food">
        <img class="Food-image" :src="food.image" :alt="food.title">
         <h5 class="Food-title">{{food.title}}</h5>
    </div>
 
</template>

<script>
export default {
    props : {
        food : {
            type : Object
        }
    }
}
</script>

<style>
    .Food{
        display: inherit;
        flex-direction: column;
        width: 100%;
        align-items: center;
        justify-content: center;
        position: relative;
        margin: 0;
        padding: 0;
    }
    .Food-title{
        text-align: center;
        margin: 0;
        padding: 0;
        position: absolute;
        bottom: 5%;
        left: 0;
        right: 0;
    }
    .Food-image{
        max-width: 150px;
        max-height: 150px;
        width: 100%;
        height: 100%;
        position: relative;
        top: 0;
    }
</style>