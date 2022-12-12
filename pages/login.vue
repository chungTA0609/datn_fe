<template><LoginComponent></LoginComponent></template>

<script>
import LoginComponent from '~/components/Login.vue';
export default {
  name: 'Login',
  layout: 'beforeLogin',
  components: {
    LoginComponent,
  },
};
</script>

<style></style>
