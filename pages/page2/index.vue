<template lang="pug">
div
  .container
    div
      p.title page2
      p {{ $data }}
      NuxtLink(to="/") top
</template>

<script>
import Vue from 'vue'

import Logo from '~/components/Logo.vue'

export default Vue.extend({
  asyncData() {
    return new Promise((resolve) => {
      setTimeout(() => {
        console.log('fetch');
        resolve({
          title: 'テスト'
        });
      }, 100);
    });
  },
  components: {
    Logo
  }
})
</script>

<style scoped>
.title {
  font-size: 20px;
  font-weight: 600;
}
</style>
