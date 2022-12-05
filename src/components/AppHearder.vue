<script>
import HeaderNav from "./HeaderNav.vue";
import SocialLinks from "./SocialLinks.vue";
import AppButton from "./AppButton.vue";

export default {
  components: {
    HeaderNav,
    SocialLinks,
    AppButton,
  },
  data() {
    return {};
  },
};
</script>

<template>
  <SocialLinks />
  <header class="d-flex py-3 px-4">
    <img src="../assets/cropped-Group-39-2x.png" alt="" />
    <HeaderNav />
    <div class="header-buttons">
      <AppButton />
      <button id="search">
        <i class="fa-solid fa-magnifying-glass"></i>
      </button>
    </div>
  </header>
</template>

<style lang="scss" scoped>
header {
  justify-content: space-between;
  align-items: center;
  z-index: 2;
}
.header-buttons {
  display: flex;
  align-items: center;
}
#search {
  border: none;
  background-color: white;
  color: var(--tertiary-color);
  margin-left: 30px;
}
</style>
