<script>
import JumboMain from "./JumboMain.vue";
import AppProperties from "./AppProperties.vue";
import AppMissions from "./AppMissions.vue";
import AppProjects from "./AppProjects.vue";
import AppFeedback from "./AppFeedback.vue";
import AppNews from "./AppNews.vue";

export default {
  components: {
    JumboMain,
    AppProperties,
    AppMissions,
    AppProjects,
    AppFeedback,
    AppNews,
  },
};
</script>

<template>
  <JumboMain />
  <AppProperties />
  <AppMissions />
  <AppProjects />
  <AppFeedback />
  <AppNews />
</template>

<style lang="scss" scoped></style>
