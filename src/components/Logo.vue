<template>
  <div class="Logo">
      <span class="Square"></span>
      <span class="Square"></span>
      <span class="Square"></span>
      <span class="Square"></span>
  </div>
</template>

<script>
export default {

}
</script>

<style>
.Logo{
    display: flex;
    width: 70px;
    height: 70px;
    flex-wrap: wrap;
    justify-self: center;
    align-self: center;
}


.Square{
    width: 50%;
    height: 50%;
    background-color : white;
}

.Square:nth-child(2){
    opacity: 0.75;
}
.Square:nth-child(3){
    opacity: 0.5;
}
.Square:nth-child(4){
    opacity: 0.25;
}

</style>