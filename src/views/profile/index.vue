<template>
  <div class="home">
       <customText tag="h1">Profile</customText>
    <div id="nav">
      <router-link to="/profile">Post</router-link> |
      <router-link to="/profile/igtv">IGTV</router-link> |
      <router-link to="/profile/save">Save</router-link> |
      <router-link to="/profile/tag">Tag</router-link>
    </div>

    <router-view />
  </div>
</template>

<script>
// @ is an alias to /src
import customText from "../../components/CustomText";


export default {
  name: 'Profile',
  components: {
    customText,
    },
};
</script>

<style scoped>

</style>
