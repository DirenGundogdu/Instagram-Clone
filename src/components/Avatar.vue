<template>
  <figure class="avatar">
    <img :src="src" :alt="alt" :width="size" :height="size" >
  </figure>
</template>

<script>
export default {
  name: "Avatar",
  props: {
    src: {
      type: String,
      default: 'https://cdn.thecustommotorcycle.co.uk/wp-content/uploads/2018/07/13113459/default_user.png'
    },
    alt: {
      type: String,
    },
    size: {
      type: Number,
    }


  }
};
</script>

<style scoped>
.avatar{
  padding: 2px;
  border-radius: 999px;
  display: inline-flex;

  background: linear-gradient(90deg,
  rgba(34,193,195,1) 0%,
  rgba(253,187,45,1) 100%);

  img{
    border-radius: inherit;
    border: 2px solid white;
  }


}

</style>