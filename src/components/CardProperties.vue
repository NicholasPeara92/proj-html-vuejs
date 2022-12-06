<script>
export default {
  data() {
    return {
      cards: [
        {
          icon: "fa-solid fa-gauge",
          name: "Speed Optimization",
        },
        {
          icon: "fa-solid fa-cloud",
          name: "Cloud Solutions",
        },
        {
          icon: "fa-solid fa-tablet-screen-button",
          name: "Website Design",
        },
        {
          icon: "fa-regular fa-clock",
          name: "Online Marketing",
        },
      ],
    };
  },
};
</script>
<template>
  <div v-for="card in cards" class="card mb-5">
    <i :class="card.icon"></i>
    <h4>{{ card.name }}</h4>
    <p>
      Far far away, behind the word mountains, far from the countries Vokalia
      Separated...
    </p>
  </div>
</template>

<style lang="scss" scoped>
.card {
  width: 430px;
  border: none;
  box-shadow: rgba(17, 17, 26, 0.1) 0px 8px 24px,
    rgba(17, 17, 26, 0.1) 0px 16px 56px, rgba(17, 17, 26, 0.1) 0px 24px 80px;
  padding: 40px;
  i {
    font-size: 40px;
    margin-bottom: 30px;
  }
  h4 {
    margin-bottom: 20px;
  }
}
.card:hover {
  background: linear-gradient(
    90deg,
    #0edaa0ff,
    #30dc90ff,
    #51dd81ff,
    #73df71ff,
    #94e061ff
  );
  color: white;
  transition: 0.5s;
}
</style>
