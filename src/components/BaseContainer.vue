<template>
  <div class="force p-10 flex-col w-screen h-screen items-center justify-center">
    <MikeIntro />
  </div>
</template>

<script>
import MikeIntro from './MikeIntro.vue';

export default {
  name: 'BaseContainer',
  props: {
    msg: String
  },
  components: {
    MikeIntro
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.force {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  width: 100%;
  background-image: url('../assets/bg.gif');
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
}
</style>
