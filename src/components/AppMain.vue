<script>
import JumboMain from "./JumboMain.vue";
import AppProperties from "./AppProperties.vue";
import AppMissions from "./AppMissions.vue";
import AppProjects from "./AppProjects.vue";
import AppFeedback from "./AppFeedback.vue";

export default {
  components: {
    JumboMain,
    AppProperties,
    AppMissions,
    AppProjects,
    AppFeedback,
  },
};
</script>

<template>
  <JumboMain />
  <AppProperties />
  <AppMissions />
  <AppProjects />
  <AppFeedback />
</template>

<style lang="scss" scoped></style>
