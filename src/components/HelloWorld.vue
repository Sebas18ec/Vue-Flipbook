<template>
  <div class="home">
    <flipbook class="flipbook" :pages="['./assets/1.jpg', './assets/1.jpg', './assets/1.jpg', 'URLs']"></flipbook>
  </div>
</template>

<script>
import Flipbook from '@/components/Flipbook.vue';

export default {
  name: 'HelloWorld',
  components: {
    Flipbook
  }
};

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.flipbook {
  width: 90vw;
  height: 90vh;
}

</style>
