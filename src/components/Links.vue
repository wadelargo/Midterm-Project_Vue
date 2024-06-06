<template>
    <a :class="['common-link', type]">
      {{ title }}
    </a>
  </template>
  
  <script>
  export default {
    props: {
      title: String,
      type: String,
    },
  };
  </script>
  
  <style scoped>
  a.common-link {
    position: relative; /* Add relative positioning to the link container */
    padding: 10px;
    border: 1px solid transparent;
    border-radius: 10px;
    width: 150px;
    display: inline-block;
    text-align: center;
    text-decoration: none;
    color: white;
    margin: 10px 40px;
    transition: transform 0.2s, box-shadow 0.3s, border 0.3s; /* Smooth transition for "transform", "box-shadow", and "border" */
    box-shadow: 0 0 0 transparent;
    overflow: hidden; /* Hide the pseudo-element border */
  }
  
  
  
  a.common-link::before {
    left: 0;
    top: 0;
    border-left: none;
    border-right: none;
  }
  
  a.common-link::after {
    right: 0;
    top: 0;
    border-left: none;
    border-right: none;
  }
  
    a.common-link:hover {
      transform: scale(2.1); /* Zoom in by 10% on hover */
      box-shadow: 0 0 40px pink; /* Add a glowing box shadow on hover */
      border-color: pink; /* Change border color on hover */
      color: black;
    }
  
  a.common-link:hover::before,
  a.common-link:hover::after {
    width: 50%; /* Expand the border on hover */
  }
  
  .one {
    
    background-color: BLUE;
    font-size: 30px;
  }
  
  .two {
    background-color: BLUE;
    font-size: 30px;
  }
  
  .three {
    background-color: BLUE;
    font-size: 30px;
  }
  .four {
    background-color: BLUE;
    font-size: 30px;
  }
  .five {
    background-color: BLUE;
    font-size: 30px;
  }
  .six {
    background-color: BLUE;
    font-size: 30px;
  }
  
  
  
  </style>