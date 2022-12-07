<script>
export default {
  props: {
    img: String,
    title: String,
  },
};
</script>
<template>
  <div class="news-card">
    <img :src="img" alt="" />
    <div id="news-title">
      <small>May 24, 2018 by Alex</small>
      <div class="d-flex">
        <div id="point"></div>
        <h5>{{ title }}</h5>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.news-card {
  width: calc(100% / 3);
  padding: 10px;
  position: relative;
  #news-title {
    position: absolute;
    background-color: white;
    padding: 40px 50px 20px 50px;
    width: 415px;
    left: 50px;
    bottom: -20px;
    small {
      color: lightgray;
    }
  }

  img {
    width: 100%;
    height: 360px;
    object-fit: cover;
    border-radius: 20px;
    box-shadow: 5px 5px 20px rgb(168 168 168);
  }
}
#point {
  background-color: var(--tertiary-color);
  border-radius: 50%;
  width: 10px;
  height: 10px;
  margin-right: 10px;
  align-self: center;
}
h5 {
  margin-top: 5px;
}
</style>
