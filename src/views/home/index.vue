<template>
  <div class="home">

    <div class="timeline">



        <Post/>

    </div>

    <div class="sidebar">
      <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusantium adipisci aperiam at cum cupiditate debitis deserunt doloribus dolorum enim ex hic minima modi nemo odit reprehenderit, rerum tenetur ullam vel.</p>

    </div>

  </div>
</template>

<script>

import Post from "../../components/Post";


export default {
  name: "Home",
  components: {
    Post,




  },
};
</script>

<style scoped>

.home{
  max-width: 605px;
  margin-left: auto;
  margin-right: auto;

  @media (--t) {
    max-width: none;
    display: grid;
    grid-template-columns:  1fr 295px;
    grid-gap: 30px;
  }
}

.sidebar{
  display: none;
  @media (--t) {
    display: block;
  }
}
</style>
