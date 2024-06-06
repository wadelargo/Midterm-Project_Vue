<script>
 import Buttons from "./components/Buttons.vue"
 import Messages from "./components/Messages.vue"
 import Cards from "./components/Cards.vue"
import Links from './components/Links.vue'

 export default {

  components: {
    Buttons,
    Messages,
    Cards,
    Links
  }
 }
</script>

<template>
  <div class="header">
    <h3>John Meward</h3>
  </div>
        <div class="box1">
             <h1>Buttons</h1>

            <div class="buttons">
              <Buttons type="regular" title="Regular"/>
              <Buttons type="happy" title="Happy"/>
              <Buttons type="sad" title="Sad"/>
              <Buttons type="angry" title="Angry"/>
            </div>
        </div>

        <div class="box2">
                <h1>Message Box</h1>
            <div class="message">
            
              <Messages type="regular" title="Regular: waning" />
              <Messages type="happy" title="Happy: Im sadly happy" />
              <Messages type="sad" title="Sad: Im sad huhuhu" />
              <Messages type="angry" title="Angry: nasuko ko grrrr yamate huhuhuu" />
            </div>
        </div>
        
        <div class="box3">
                <h1>Cards</h1>
        <div class="cards">
          <Cards type="one" title="My Kingdom"/>
          <Cards type="two" title="My Lord"/>
          <Cards type="three" title="My savior"/>
          <Cards type="four" title="My wife"/>
          <Cards type="five" title="My Love"/>
          <Cards type="six" title="My Boss"/>

        </div>
        </div>

        <div class="box4">
             <h1>Links</h1>

          <div class="links">
           
            <Links type="two" title="YouTube" href="https://www.youtube.com/"/>
            
            <Links type="four" title="Nkiri" href="https://nkiri.com/"/>
            <Links type="five" title="Figma" href="https://www.figma.com/"/>
            <Links type="six" title="Vue" href="https://www.mobilelegends.com/en"/>
            <Links type="one" title="Facebook" href="https://www.facebook.com/"/>
            <Links type="three" title="Google" href="https://www.google.com/"/>
          </div>
        </div>
   
</template>
<style scoped>

.links {
  padding: 20px;
  margin-left: 180px;
}
.box1 {
  padding: 20px;
  margin: 0;
  background-color: white;
  
}
.box2 {
  margin: 0;
  padding: 20px;
  background-color: white;
}
A.box3 {
  margin: 0;
  padding: 20px;
  
  background-color: white;
}
.box4 {
  margin: 0;
  padding: 20px;
  background-color: white;
}
.header {
  padding: 17px;
  margin: 0;
  background-color: rgba(128, 128, 128, 0.493);
   box-shadow: 10px 10px 50px 3px skyblue inset;
  color: white;
}
h3 {
  margin-left: 30px;
  font-size: 30px;
  color: blueviolet;
  text-align: center;
}
h1 {
  text-align: center;
  color: black;
}
.buttons {
  margin-left: 200px;
  

}

h1 {
}
.message {

 background-color: rgba(128, 128, 128, 0.493);
 padding: 40px;
 border-radius: 10px;
 display: flex;
 box-shadow: 10px 10px 70px 7px black inset;


}
.cards {
  padding: 20px;
  text-align: center;
  box-shadowe: rgb(34, 8, 8)
  
}
</style>