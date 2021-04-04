<template>
  <div class="home">
       <customText tag="h1">Profile TAG</customText>
    <homeIcon/>
  </div>
</template>

<script>
// @ is an alias to /src
import customText from "../../components/CustomText";


export default {
  name: 'ProfileTag',
  components: {
    customText,
    },
};
</script>

<style scoped>

</style>
