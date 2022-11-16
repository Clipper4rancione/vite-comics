<script>
import AppHeader from "./components/AppHeader.vue";
import AppJumbo from "./components/AppJumbo.vue";
import AppMain from "./components/AppMain.vue";
import BlueMenu from "./components/BlueMenu.vue";
import AppFooter from "./components/AppFooter.vue";
import AppFooterBot from "./components/AppFooterBot.vue";

export default {
  name: "Vue",
  components: {
    AppHeader,
    AppMain,
    AppFooter,
    BlueMenu,
    AppFooterBot,
    AppJumbo,
  },
};
</script>

<template>
  <AppHeader />
  <AppJumbo />
  <AppMain />
  <BlueMenu />
  <AppFooter />
  <AppFooterBot />
</template>


<style lang="scss">
@use "./styles/partial/variables" as *;
@use "./styles/general.scss" as *;
</style>