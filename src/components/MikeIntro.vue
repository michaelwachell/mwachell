

<template>
  <div class="hero-container  rounded">
    <div class="inner-container">
      <div class="me-image-container float-around rounded-full">
        <!-- <img src="../assets/Mike.jpg" class="me-image" /> -->
      </div>
      <div class="">
        <h1 class="text-slate-800 mb-10">Hi, my name is <span class="font-bold">Mike</span> &#128075;</h1>
        <blockquote class="text-slate-800">
          <h2>
            I am a <span class="text-teal-600 font-bold">leader &#127939;, </span> a <span
              class="text-teal-600 font-bold">software
              engineer
              &#128187;, </span> and a
            <span class="text-teal-600 font-bold">creative &#127925;. </span>
          </h2>
          <div class="links-out">
            <a class="fa-brands fa-github cpointer"></a>
            <a class="fa-brands fa-linkedin cpointer"></a>
            <a class="fa-brands fa-twitter cpointer"></a>
            <a class="fa fa-solid fa-scroll cpointer jiggle-me"> </a>
            <!-- <a class="fa-brands fa-github cpointer " v-tooltip="Github"></a>
                 <a class="fa-brands fa-linkedin cpointer" v-tooltip="LinkedIn"></a>
                      <a class="fa-brands fa-twitter cpointer" v-tooltip="Twitter"></a>
                      <a class="fa fa-solid fa-scroll cpointer jiggle-me" v-tooltip="Resume">  </a> -->
          </div>

        </blockquote>
      </div>
      <div>
        <!-- add social links for github and linkedin -->

      </div>

    </div>
  </div>
</template>

<script>
// import {v-tooltip} from 'vue-tooltip';

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
  width: 80%;
  height: 80%;

  padding: 20px;
  // background left to right gradient transparent to white
  background: linear-gradient(to bottom, rgba(0, 0, 0, 0) 25%, #fff);

  @media #{$tabletAndLarger} {
    background: linear-gradient(to right, rgba(0, 0, 0, 0) 25%, #fff);
    width: 80%;
    height: 60%;

  }

}

.inner-container {
  width: 100%;
  height: 100%;
  @include col-between;

  @media #{$tabletAndLarger} {
    @include row-evenly;

  }
}

.me-image-container {
  // write a circular clipping mask for this image
  width: 65vw;
  height: 60vw;

  @media #{$tabletAndLarger} {
    width: 30vw;
    height: 30vw;

  }

  // add thick drop shadow to the image
  box-shadow: 100px 100px 300px rgba(0, 0, 0, 1);
  border: 10px solid black;

  // clip the image to a circle

  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
  background-image: url(../assets/Mike.jpg);


}

// create animation that spins element once and grows the element one times over 9 seconds


.jiggle-me {
  animation: jiggle 8s linear infinite;
}

// create a flex row class
.links-out {
  @include row-start;
  width: 100%;
  margin-top: 40px;

  a {
    transition: all 0.3s linear;
    margin-right: 5%;

    &:hover {
      color: #fff;
      transform: scale(1.2);
      transition: all 0.3s linear;

    }
  }
}
</style>
