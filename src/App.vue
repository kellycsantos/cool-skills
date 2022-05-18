<template>

    <div id="container">
      <MenuPrincipal/>
      <EmailCapture/>
      <CardsBeneficios/>
      <router-view/>
    </div>

</template>

<script lang="ts">
import Vue from 'vue';
import MenuPrincipal from './components/MenuPrincipal.vue'
import EmailCapture from './components/EmailCapture.vue'
import CardsBeneficios from './components/CardsBeneficios.vue'


export default Vue.extend({
  name: 'App',
    components: {
  
      MenuPrincipal,
      EmailCapture,
      CardsBeneficios,
    },
    
  

  data: () => ({
    //
  }),
});
</script>



<style >
   *{
    margin: 0;
    padding: 0;
    outline: none;
    box-sizing: border-box;
    text-decoration: none;
  }
  body{
    background: #594ec4 ;
    padding: 0 50px;
    display: flex;
    justify-content: center;
  }

  #container{
    max-width: 1300px;
  }


 
</style>


