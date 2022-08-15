<template>
  <div class="w-64">
    <img src="../assets/Mike.jpg" />
    <h2>Hi, My name is Mike</h2>
    <blockquote>
      I am a <span class="text-teal-200">Leader</span> a <span>software engineer</span> and a <span>creator</span>
    </blockquote>
  </div>
</template>

<script>
export default {
  name: 'MikeIntro',
  props: {
    msg: String
  }
};
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
