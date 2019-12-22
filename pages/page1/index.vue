<template lang="pug">
div
  .container
    div
      p page1
      Logo
      div
        button(@click="$router.back()") back
</template>

<script>
import Vue from 'vue'

import Logo from '~/components/Logo.vue'

export default Vue.extend({
  components: {
    Logo
  },
  transition: 'fade'
})
</script>

<style>
</style>
