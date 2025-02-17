<template>
  <div>
    <the-header></the-header>
    <router-view />
  </div>
</template>

<script>
import TheHeader from './components/header/TheHeader.vue';

export default {
  components: {
    TheHeader,
  },
};
</script>
