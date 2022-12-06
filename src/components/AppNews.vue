<script>
import NewsCard from "./NewsCard.vue";
import AppSpacer from "./AppSpacer.vue";
import DarkButton from "./DarkButton.vue";

export default {
  components: {
    NewsCard,
    AppSpacer,
    DarkButton,
  },
  data() {
    return {
      news: [
        {
          img: "src/assets/serious-businesswoman-with-documents-talking-on-P9Q6LX6-1024.jpg",
          title: "Marketing Ideas",
        },
        {
          img: "src/assets/Businessman-at-the-desk-in-his-office-resting--1024x768.jpg",
          title: "Rest During Working Hours",
        },
        {
          img: "src/assets/person-with-long-curly-hair-PZ99QM2-2x.jpg",
          title: "Develop Your Startup Idea",
        },
      ],
    };
  },
};
</script>
<template>
  <section>
    <h3>Latest News & Our<mark>Blog</mark></h3>
    <AppSpacer id="spacer" />
    <div class="d-flex pt-5 pb-5">
      <NewsCard
        v-for="content in news"
        :img="content.img"
        :title="content.title"
      />
    </div>
    <div id="btn">
      <DarkButton />
    </div>
  </section>
</template>

<style lang="scss" scoped>
section {
  background-color: var(--secondary-color);
  padding-top: 200px;
  position: relative;
  #spacer {
    position: absolute;
    left: 50%;
    top: 280px;
  }
  h3 {
    text-align: center;
    font-size: 42px;
    font-weight: bold;
  }
}
mark {
  background-color: inherit;
  color: var(--tertiary-color);
}
#btn {
  text-align: center;
  padding-top: 30px;
  padding-bottom: 200px;
}
</style>
