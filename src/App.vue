<script>
import AppHeader from "./components/AppHeader.vue";
import AppFooter from "./components/AppFooter.vue";
import AppMain from "./components/AppMain.vue";
import BlueMenu from "./components/BlueMenu.vue";
import AppFooterBot from "./components/AppFooterBot.vue";

export default {
  name: "Vue",
  components: {
    AppHeader,
    AppMain,
    AppFooter,
    BlueMenu,
    AppFooterBot,
  },
};
</script>

<template>
  <AppHeader />
  <AppMain />
  <BlueMenu />
  <AppFooter />
  <AppFooterBot />
</template>


<style lang="scss">
@use "./styles/partial/variables" as *;
@use "./styles/general.scss" as *;
</style>