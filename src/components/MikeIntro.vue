<template>
  <div class="hero-container">
    <div class="">
      <div class="me-image-container float-around rounded-full">
        <!-- <img src="../assets/Mike.jpg" class="me-image" /> -->
      </div>
      <div class="">
        <h2 class="text-slate-500">Hi, My name is Mike</h2>
        <blockquote class="text-slate-600">
          I am a <span class="text-teal-500 animate-pulse">Leader</span> a <span class="text-teal-500">software
            engineer</span> and a
          <span class="text-teal-500">creator</span>
        </blockquote>
      </div>

    </div>
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
<style scoped lang="scss">
.hero-container {
  @include row-center;
  width: 50%;

}

.me-image-container {
  // write a circular clipping mask for this image
  width: 300px;
  height: 300px;
  // add thick drop shadow to the image
         box-shadow: 100px 100px 300px rgba(0, 0, 0, 1);
        border: 4px solid black;

  // clip the image to a circle
  
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
  background-image: url(../assets/Mike.jpg);


}

.me-image {


}
</style>
