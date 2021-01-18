<template>
    <div class="Food">
        <img class="Food-image" :src="food.image" :alt="food.title" width="150" height="150">
        <p class="Food-title">{{food.title}}</p>
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
        height: auto;
        align-items: center;
        justify-content: center;
        margin: 0;
        padding: 0;
        cursor: pointer;
        transition: 1s cubic-bezier(0.23, 1, 0.320, 1);
    }
    .Food-title{
        width: 90%;
        margin: 0;
        padding: 0;
        font-size: 1.25em;
        text-align: center;
    }
    .Food-image{
        max-width: 150px;
        max-height: 150px;
        width: 90%;
        height: 50%;
        align-self: center;
        justify-self: center;
        
    }

    .Food:hover{
        background: rgba(255,192,85);
        transform: scale(1.35,1.35);
        color: white;
    }

    .Food:hover .Food-title{
        margin-top: -10px;
        padding-bottom: 10px;
    }
</style>