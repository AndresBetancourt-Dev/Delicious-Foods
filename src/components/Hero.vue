<template>

  <div class="Hero">
           <Header/>
    <div class="Content">
        <div class="Grid">
          <div class="Form">
             <h1 class="Form-title">DELICIOUS FOOD</h1>
          <p class="Form-text">Delicious food, color, aroma and taste, What are you waiting for?</p>
          <form class="Form-container">
            <label for="email">Email</label>
            <input type="text" class="Form-input" name="email" id="email" placeholder="rwds@example.com"> 
            
            <input type="submit" class="Form-button" value="Confirm">
          </form>
          </div>
        </div>
        <div class="Grid">
          <img src="../assets/images/pan.webp" class="Egg" alt="Egg in a Pan"/>
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
  min-height: 77.5vh;
  display: flex;
  flex-direction: column;
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
  font-family: 'Morn',sans-serif;
}

.Form-text{
  font-family: 'Mazzard H';
  font-weight: bold;
}


label[for="email"]{
  font-size: 0;
}

.Form-input, .Form-button{
  padding: 1em;
  border: none;
  outline: none;
  border-radius: 30px;
  box-shadow: 0px 0px 5em rgba(0,0,0,.5);
  font-family: 'Myriad Pro Bold',sans-serif;
  font-size: 1em;
}

.Form-input{
  padding: 15px 3em;
  width: 65%;
}

.Form-input::placeholder{
  color: rgba(0,0,0,.2);
}

.Form-button{
  margin-left: 10px;
  padding: 15px;
  width: 25%;
  cursor: pointer;
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

@media screen and (max-height: 700px) {
  .Egg{
    max-width: 400px;
  }
}

@media screen and (max-width: 600px){
  .Form-container{
    display: flex;
    flex-wrap: wrap;
    justify-items: flex-start;
  }
  .Form-input, .Form-button{
    width: 100%;
    margin: 1em;
  }
}

@media screen and (max-width: 950px ) {
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
    max-width: 40%;
    max-height: 300px;
    align-self: center;
    justify-self: center;
  }
  .Shadow{
    align-self: center;
    justify-self: center;
    left: 30%;
    bottom: 30%;
  }
}

@media screen and (min-width : 1660px) {
  .Shadow{
    max-width: 200px;
    max-height: 200px;
     box-shadow: 0px 0px 10em rgba(0,0,0,.3), 0px 0px 10em rgba(0,0,0,.45), 0px 0px 10em rgba(0,0,0,.55), 0px 0px 10em rgba(0,0,0,.6);
     left: 30%;
  }
     
}

</style>