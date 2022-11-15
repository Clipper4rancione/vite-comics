<script>
import AppHeader from "./components/AppHeader.vue";
import AppFooter from "./components/AppFooter.vue";
import AppMain from "./components/AppMain.vue";

export default {
  name: "Vue",
  components: {
    AppHeader,
    AppMain,
    AppFooter,
  },
};
</script>

<template>
  <div class="container">
    <AppHeader />
  </div>
  <AppMain />
  <AppFooter />
</template>


<style lang="scss">
@use "./styles/general.scss" as *;
</style>