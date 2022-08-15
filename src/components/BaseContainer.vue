<template>
  <div class="w-64">
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
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
