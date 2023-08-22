<!-- eslint-disable vue/multi-word-component-names -->
<template>
    <div class="flipbook-container">
      <flipbook :pages="pages"
        v-slot="flipbook">
        <button @click="flipbook.flipLeft">Página Anterior</button>
        <button @click="flipbook.flipRight">Página Siguiente</button>
      </flipbook>
    </div>
  </template>
  
  <script>
  
  import Flipbook from 'flipbook-vue';
  
  export default {
    // eslint-disable-next-line vue/multi-word-component-names
 
    components: {
      Flipbook
    },
    props: {
      pages: {
        type: Array,
        required: true
      }
    }
  };
  </script>
  
  <style>
  /* Estilos personalizados para tu componente Flipbook */
  .flipbook-container.flipbook {
    width: 900px;
    height: 450px;
    display: flex;
    position: relative;
    /*flex-direction: column;*/
    /*align-items: center;
    justify-content: center;    */
  }

  .flipbook-container.flipbook>div{
    margin: 0 auto;
  }

  .flipbook-container.flipbook>div>div{
    width: 900px;
    height: 450px;
  }

  
  
/*.flipbook {
  width: 90vw;
  height: 90vh;
}*/
</style>
  