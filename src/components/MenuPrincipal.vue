<template>
    <div id="container">

        <span class="icon-home">
            <h1>D</h1>
        </span>
        <span>
        <router-link to="/">Home</router-link>
        <router-link to="/about">Sobre</router-link>
        <router-link to="/">Topicos</router-link>
        <router-link to="/">Contatos</router-link>
        </span>
    </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
    name:'MenuPrincipal'
})
</script>

<style>

</style>

<style scoped>
    #container{
        height: 80px;
        display: flex;
        align-items: center;
        justify-content: space-between;
    }
    a{
        color: aliceblue;
        font-size: 18px;
        margin: 0 10px 0 10px;

    }
    .icon-home{
        color: aqua;
    }
</style>