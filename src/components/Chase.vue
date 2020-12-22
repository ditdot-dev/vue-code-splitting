<template>
  <profile :name="'chase'" :image="require('../assets/images/chase.jpg')">
    <ul>
      <li>Loves art and truffels</li>
      <li>Undercover agent</li>
      <li>A bit of a womanizer</li>
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