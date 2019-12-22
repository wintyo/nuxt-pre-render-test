<template lang="pug">
div
  .container
    div
      p page2
      NuxtLink(to="/") top
</template>

<script>
import Vue from 'vue'

import Logo from '~/components/Logo.vue'

export default Vue.extend({
  components: {
    Logo
  }
})
</script>

<style>
</style>
