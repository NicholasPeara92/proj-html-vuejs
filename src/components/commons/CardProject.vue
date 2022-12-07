<script>
export default {
  props: {
    img: String,
    description: String,
    type: String,
  },
};
</script>

<template>
  <div class="project-card">
    <img :src="img" alt="" />
    <div id="veil">
      <h6>{{ description }}</h6>
      <small>{{ type }}</small>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.project-card {
  position: relative;
  width: calc(100% / 4);
  img {
    width: 100%;
    border-radius: 10px;
  }
  #veil {
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    background: linear-gradient(
      90deg,
      #0edaa0ff,
      #30dc90ff,
      #51dd81ff,
      #73df71ff,
      #94e061ff
    );
    opacity: 0.8;
    color: white;
    display: none;
    padding: 70% 20px 20px 40px;
    border-radius: 10px;
    h6 {
      font-size: 20px;
    }
  }
}
.project-card:hover {
  scale: 1.1;
  z-index: 3;
}
.project-card:hover #veil {
  display: block;
}
</style>
