<template>

  <div class="Hero">
           <Header/>
    <div class="Content">
        <div class="Grid">
          <div class="Form">
             <h1 class="Form-title">DELICIOUS FOOD</h1>
          <p class="Form-text">Delicious food, color, aroma and taste, What are you waiting for?</p>
          <form>
            <label for="email">Email</label>
            <input type="text" class="Form-input" name="email" id="email" placeholder="your-email@example.com"> 
            
            <input type="submit" value="Confirm">
          </form>
          </div>
        </div>
        <div class="Grid">
          <img src="../assets/pan.png" class="Egg" alt="Egg in a Pan"/>
          <div class="Shadow"></div>
        </div>
    </div>
  </div>
  
</template>

<script>
import Header from "./Header"
export default {
    components : {
        Header
    }
}
</script>

<style>
.Hero{
  min-height: 80vh;
  display: block;
  background: radial-gradient(rgb(247,103,48),rgb(247,103,48),rgb(248,61,30));
}

.Content{
  display: grid;
  width: 100%;
  height: auto;
  min-height: 60vh;
  grid-template-columns: repeat(2,1fr);
}

.Grid{
  width: 100%;
  height: 100%;
  display: inherit;
  align-items: center;
  justify-items: center;
  position: relative;
  text-align: left;
}

.Form{
  width: 65%;
  justify-self: end;
}

.Form-title, .Form-text{
  color: white;
}

.Form-title{
  font-size: 8vw;
  line-height: 1em;
  margin: 0;
}

label[for="email"]{
  font-size: 0;
}

.Form-input, .Form-button{
  padding: 1em;
  border: none;
  outline: none;
  border-radius: 20px;
  box-shadow: 0px 5px 40px rgba(0,0,0,.5);
}

.Egg{
  max-width: 100%;
  height: auto;
  position: absolute;
  z-index: 5;
}

.Shadow{
  position: absolute;
  width: 12.5vw;
  height: 12.5vw;
  border-radius: 50%;
  bottom: 22.5%;
  left: 15%;
  background: rgba(0,0,0,.485);
  box-shadow: 0px 0px 10vw rgba(0,0,0,.3)
  ,0px 0px 10vw rgba(0,0,0,.45)
  ,0px 0px 10vw rgba(0,0,0,.55)
  ,0px 0px 10vw rgba(0,0,0,.6)
  ;
}

@media screen and (max-width: 850px ) {
  .Content{
    grid-template-columns: 1fr;
    height: auto;
    justify-items: center;
    align-items: center;
    min-height: 100vh;
  }

  .Form{
    justify-self: center;
  }

  .Egg{
    max-width: 50%;
    align-self: center;
    justify-self: center;
  }
  .Shadow{
    align-self: center;
    justify-self: center;
    left: 30%;
  }
}

</style>