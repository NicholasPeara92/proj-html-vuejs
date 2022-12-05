<script>
import AppHeader from "./components/AppHearder.vue";
import AppMain from "./components/AppMain.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
  components: {
    AppHeader,
    AppMain,
    AppFooter,
  },
};
</script>

<template>
  <div class="my-container">
    <AppHeader />
    <AppMain />
    <AppFooter />
  </div>
</template>

<style lang="scss">
@import "./style/global.scss";
.my-container {
  width: 1536px;
  margin: auto;
}
</style>
