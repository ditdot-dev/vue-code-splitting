<template>
  <profile :name="'marshall'" :image="require('../assets/images/marshall.jpg')">
    <ul>
      <li>Cute as a button</li>
      <li>Your best friend forever</li>
      <li>Founder of a dog dating app</li>
    </ul>
  </profile>
</template>

<script>
  import Profile from './Profile.vue'

  export default {
    components: {
        Profile
    }
  }
</script>

<style>

</style>