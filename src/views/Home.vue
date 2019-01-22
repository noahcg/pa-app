<template>
  <div class="container">
    <MainHub msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import MainHub from '@/components/MainHub.vue';

export default {
  name: 'home',
  components: {
    MainHub,
  },
};
</script>
