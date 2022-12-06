<script>
import JumboMain from "./JumboMain.vue";
import AppProperties from "./AppProperties.vue";
import AppMissions from "./AppMissions.vue";
import AppProjects from "./AppProjects.vue";

export default {
  components: {
    JumboMain,
    AppProperties,
    AppMissions,
    AppProjects,
  },
};
</script>

<template>
  <JumboMain />
  <AppProperties />
  <AppMissions />
  <AppProjects />
</template>

<style lang="scss" scoped></style>
