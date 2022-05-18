<template>
    <div id="container">
        <span class="informacoes" 
              v-for="beneficio,index in beneficios" :key="index">
            <img class="icons" :src="require(`../assets/${beneficio.icon}.png`)">
            <h3>{{beneficio.title}}</h3>
            <small>{{beneficio.description}}</small>
        </span>
    </div>

</template>


<script lang="ts">
import Vue from 'vue'


export default Vue.extend({
    name:'CardsBeneficios',
    data(){
        return{
        beneficios:[
            {
                title:"Live Chating",
                description: "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Velit debitis amet fugit nesciunt eius",
                icon: "Message_perspective_matte_s"
            },
            {
                title:"Question Answer",
                description: "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Velit debitis amet fugit nesciunt eius",
                icon: 'Envelope_perspective_matte_s'
            },
            {
                title:"Right Feedback",
                description: "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Velit debitis amet fugit nesciunt eius",
                icon: "Like_perspective_matte_s"
            }
        ],
        }
    }
})
</script>

<style>

</style>

<style scoped>
    #container{
        height: 80px;
        display: flex;
        flex-direction: column;
        align-items: center;
    }

    .informacoes{
        background: whitesmoke;
        width: 215px;
        height: 170px;
        border-radius: 20px;
        padding: 20px;
        margin: 20px 0;
        display: flex;
        flex-direction: column;
        justify-content: center;
    }

    .icons{
        width: 100px;
        margin-top: -60px;
        align-self: center;
    }

  

    @media screen and (min-width:768px) {
    #container{
        flex-direction: row;
        align-items: center;
        justify-content: space-around;
        margin: 50px;
    }
      .icons{
        width: 80px;
        margin-top: -100px;
        align-self: center;
    }

    }
</style>