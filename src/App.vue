<template>
  <div class="home">
    <flipbook class="flipbook" :pages="[
       'https://www.futbolecuador.com/imagenes/images/thumb640/8060a06fe9d24690d117dac5b065fc36.jpg',
       'https://www.futbolecuador.com/imagenes/images/thumb640/6795cbe58e5f495073efaa4f61ca8615.jpg',
       'https://www.futbolecuador.com/imagenes/images/thumb640/9808bead3c2a5f270faf67a2381712c5.jpeg',
       'https://www.futbolecuador.com/imagenes/images/thumb640/6f746c6e848feb9055fc0d85e80ffcde.jpg',
       'https://www.futbolecuador.com/imagenes/images/thumb640/0b3ef29091998279d52312bead978a58.jpeg',
       'https://www.futbolecuador.com/imagenes/images/thumb640/81e5075161e2305a6818c4d799a82b60.jpeg',
       'https://www.futbolecuador.com/imagenes/images/thumb640/71e795b2a8e6976ec86fc31fdde049c7.jpg',
       ]" :zooms="2" :singlePage="true" :centering='true'></flipbook>
  </div>
</template>

<script>


import Flipbook from '@/components/Flipbook.vue';

export default {
  name: 'App',
  components: {
    Flipbook
  }
}
</script>

<style>

.flipbook {
  width: 90vw;
  height: 90vh;
}
</style>
