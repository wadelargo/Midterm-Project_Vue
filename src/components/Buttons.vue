<script>
export default {
    props: {
        title: String,
        type: String
    }
}
</script>
<template>
    <button :class="type">
        {{ title }}
    </button>
</template>

<style scoped>
 button {
    padding: 20px;
    width: 310px;
    margin-left: 45px;
    box-shadow: 10px 10px 40px 3px black;
    cursor: pointer;
 
  
 }
 button:hover {
   box-shadow: 0 0 20px black;
   color: black;
 }

 .regular {
    font-size: 25px;
    background-color: rgba(0, 0, 255, 0.835);
    color: white;
    border: 1px solid blue;
    border-radius: 10px;


 }
 .regular:hover {
    background-color: blue;
    transition: 0.3s;
 }

 .happy {
    font-size: 25px;
    background-color: rgba(0, 128, 0, 0.787);
    color: white;
    border: 2px solid green;
    border-radius: 10px;
 }
.happy:hover {
    background-color: green;
    transition: 0.3s;
}

 .sad {
    font-size: 25px;
    background-color: rgba(253, 253, 12, 0.674);
    color: black;
    border: 2px solid rgb(151, 151, 8);
    border-radius: 10px;

 }

 .sad:hover {
    background-color: yellow;
    transition: 0.3s;
 }

 .angry {
    font-size: 25px;
    background-color: rgba(255, 0, 0, 0.724);
    color: white;
    border: 2px solid red;
    border-radius: 10px;
 }
 .angry:hover {
    background-color: red;
    transition: 0.3s;
 }

</style>