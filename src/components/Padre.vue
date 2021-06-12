<template>
    <div class="padreDiv">
        <h2>Componente Padre:</h2>
        <Hijo v-for="(item, index) of itemsPadre" :key="index" :items="item" :numero="numeroPadre"></Hijo>  
    </div>
</template>


<script>
import Hijo from "./Hijo"

export default{
    name: "Padre",
    components: {Hijo},
    data(){
        return {
            numeroPadre: 0,
            itemsPadre: [1,2,3]
        }
    }
}
</script>


<style>
.padreDiv{
    background: #D7DBDF;
    border:3px solid #40B983;
}
</style>