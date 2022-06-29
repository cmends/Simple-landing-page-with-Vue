<template>
  <button> {{text}} </button>
</template>

<script>
export default {
    name: "AppButton",
    props:["text"],
    
}
</script>

<style scoped>
button{
    margin: 30px auto;
    display: block;
    padding: 8px;
    font-size: 16px;
    background-color: gold;
    margin-top: 20px;
}
</style>
