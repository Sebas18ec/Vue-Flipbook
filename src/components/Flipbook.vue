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
  .flipbook-container {
    width: 150%;
    height: 150%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    transform: scale(4) !important;
  }
  </style>
  