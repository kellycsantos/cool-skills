<template>
    <div id="container">
        <span id="info">
            <span class="info">
                <h1>De um Glow up nas suas habilidates de comunicação.</h1>
            <span class="form">    
                    <form>
                        <input type="email" required placeholder="Email">
                        <input type="submit" value="Junte-se">
                    </form>
            </span>        
            </span>
            <span class="image-girl">
                <img src="../assets/images/girl.png">
            </span>
        </span>    
    </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
    name:'EmailCapture'
})
</script>

<style>

</style>

<style scoped>
    #container{
        display: flex;
        flex-direction: column;
        align-items: center;
    }

    .info{
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        margin-top: 10px;
    }

    .info h1{
        color: blanchedalmond;
    }

    .image-girl{
        display: flex;
        justify-content: center;
    }
    .image-girl img{
        width: 350px;        
    }

    .form{

        display: flex;
        text-align: center;
        margin: 15px 0 -5px 0;
    }

    input{
        border: 1px solid white;
        border-radius: 12px ;
        height: 45px;
        padding: 0 10px;
    }
    input[type="email"]{
        width: 70vw;
        display: block;
        color: whitesmoke;
        margin: 15px;
    }
    input[type="submit"]{
        background: whitesmoke;
    }   

    @media screen and (min-width:768px) {
    #container{
        display: flex;
        align-items: center;
        justify-content: space-between;
        
    }

    #info{
        display: flex;
    }

    .info{
        height: auto;
    }
    a{
        color: aliceblue;
        font-size: 18px;
        margin: 0 10px 0 10px;

    }


    input{
        border: 1px solid white;
        border-radius: 12px ;
        height: 45px;
        padding: 0 10px;
    }
    input[type="email"]{
        width: 270px;
        margin-right: 10px;
    }
    input[type="submit"]{
        background: whitesmoke;
    }
    }
</style>