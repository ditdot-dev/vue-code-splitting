<template>
  <div class="tabs-container">
    <div class="tabs">
      <button 
        v-for="(pup, index) in pups"
        @click="setUserName(pup)" 
        :key="index" 
        class="tab" 
        :class="[pup, {active: user === pup}]" 
      >
        {{ pup }}
      </button>
    </div>
    <component :is="userProfile"></component>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        pups: ['Chase', 'Marshall','Rider'],
        user: 'Chase'
      }
    },
    computed: {
      userProfile() { 
        // We must explicitly use this.user inside the computed property for this to work
        const user = this.user
        return () => import( /* webpackChunkName: "[request]" */ `./components/${user}.vue`)
      }
    },
    methods: {
      setUserName(pup) {
        this.user = pup
      }
    }
  }
</script>

<style>
  @import './assets/css/pups.css';
  @import url('https://fonts.googleapis.com/css2?family=Lato:wght@400;700;900&display=swap');
</style>
