<template>
    <div class="hijoDiv" >
        <h4>Item {{items}}:</h4>
        <button @click="numero++">{{numero}}</button>
    </div>
</template>


<script>
export default{
    name: "Hijo",
    props: ['numero', "items"]
}
</script>

<style>
.hijoDiv{
    background: white;
    width: 30%;
    margin:auto;
    border:3px solid #40B983;   
    margin-bottom: 20px;
}

button{
    background: #40B983;
    border:none;
    border-radius: 5px;
    padding:10px;
    margin-bottom: 10px; 
}
</style>