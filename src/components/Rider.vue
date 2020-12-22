<template>
  <profile :name="'rider'" :image="require('../assets/images/rider.jpg')">
    <ul>
      <li>Playing with a ball</li>
      <li>Playing with a ball</li>
      <li>Playing with a ball</li>
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