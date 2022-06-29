<template>
    <div class="card-container">
        <div class="card">
            <figure>
                <img :src="cardImage" alt="">
            </figure>
            <h1>{{cardHeading}}</h1>
            <p>{{cardText}}</p>
        </div>
    </div>
</template>

<script>
export default {
    name: "AppCard",
props:["cardText","cardHeading","cardImage"],
}
</script>

<style scoped>


.card{
    height: 300px;
    width: 300px;
    /* background: rgb(226, 218, 218); */
    border-radius: 10px;
    /* display: block; */
    /* margin-right: 100px; */ 
}
p{
    color:black;
    font-size: 15px;
}
h1{
    color: rgb(228, 164, 81);
    font-size: 20px;
    margin: 10px;
}
img {
    width: 370px;
    height: 300px;
   
}

</style>