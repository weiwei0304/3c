<template>
  <div class="min-h-screen">
    <the-header></the-header>
    <div class="pt-[160px]">
      <router-view />
    </div>
    <the-footer></the-footer>
  </div>
</template>

<script>
import TheHeader from './components/header/TheHeader.vue';
import TheFooter from './components/footer/TheFooter.vue';

export default {
  components: {
    TheHeader,
    TheFooter,
  },
};
</script>

<style>
:root {
  scroll-padding-top: 100px;
}
</style>
