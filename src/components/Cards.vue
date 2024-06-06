<template>
    <div class="card">
      <div class="card-header">
        <h1>1</h1>
      </div>
      <div class="sudCard">
  
        <div class=content>
            <text :class="type">
              {{ title }}
            </text>
            
        </div> 
       <div class="buttons">
        <Buttons style="flex: 1" title="like" type="regular" />
        <Buttons style="flex: 1" title="dislike" type="angry" />
       </div>
     </div>
    </div>
  </template>
  
  <script>
  import Buttons from './Buttons.vue'
  
  export default {
      props: {
          title: String,
          type: String
      },
  
    components: {
      Buttons
    }
  };
  </script>
  
  <style scoped>
  h1 {
    margin-top: 5px;
    color: white;
  }
  .one {
    font-size: 40px;
    padding: 20px;
    border-radius: 10px;
    background-color: skyblue;
  }
  .two {
    font-size: 40px;
    padding: 20px;
    border-radius: 10px;
    background-color: rgba(255, 0, 0, 0.795);
  }
  
  .three {
    font-size: 40px;
     padding: 20px;
    border-radius: 10px;
    background-color: yellow;
  }
  
  .four {
    font-size: 40px;
     padding: 20px;
    border-radius: 10px;
    background-color: gray;
  }
  .five {
    font-size: 40px;
     padding: 20px;
    border-radius: 10px;
    background-color: violet;
  }
  .six {
    font-size: 40px;
     padding: 20px;
    border-radius: 10px;
    background-color: green;
  }
  .card {
    background-color: #f7f7f7;
    border: 1px solid #e0e0e0;
    border-radius: 5px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    display: inline-block;
    flex-direction: column;
    transition: transform 0.2s;
    overflow: hidden;
    width: 500px;
    margin: 10px;
    cursor: pointer;
    flex-wrap: wrap;
  }
  .content {
    padding: 100px;
    text-align: center;
  }
  .regular, .angry {
    flex: 1; /* Equal width for both buttons */
    margin: 20px 0px;
    
   
    
  }
  .card:hover {
    transform: translateY(-5px);
  }
  
  .buttons {
    padding: 20px;
    display: flex;
    justify-content: space-between;
  }
  
  .card-header {
    height: 40px;
    background-color: black;
    overflow: hidden;
    position: relative;
  }
  
  .card-header img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: center top;
  }
  
  .card-content {
    padding: 100px;
    
  }
  
  h3 {
    font-size: 24px;
    margin: 0;
  }
  
  p {
    font-size: 16px;
    color: #555;
    margin: 5px 0;
  }
  .sudCard {
    background-color: gray;
  }
  </style>
  