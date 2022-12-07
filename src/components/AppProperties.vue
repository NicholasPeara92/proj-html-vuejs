<script>
import CardProperties from "./commons/CardProperties.vue";
import AppButton from "./commons/AppButton.vue";

export default {
  components: {
    CardProperties,
    AppButton,
  },
};
</script>
<template>
  <section>
    <div class="title-section">
      <h2>
        We Are Here To <br />
        Make Your <mark>Website</mark><br />
        Look More <mark>Elegant</mark><br />
        And Stylish!
      </h2>
      <AppButton id="section-btn" />
    </div>
    <div class="card-section"><CardProperties /></div>
  </section>
</template>

<style lang="scss" scoped>
section {
  display: flex;
  justify-content: space-between;
  margin-top: -80px;
  background-color: white;
  padding-top: 140px;
  margin-bottom: 100px;
}
.title-section {
  width: 35%;
  padding-right: 50px;
  padding-left: 20px;
  position: relative;
  h2 {
    font-size: 45px;
    line-height: 60px;
    font-weight: bold;
    padding-top: 60px;
  }
}
mark {
  background-color: white;
  color: var(--tertiary-color);
}
.card-section {
  display: flex;
  flex-wrap: wrap;
  width: 65%;
  justify-content: space-around;
}
.title-section::after {
  content: "";
  position: absolute;
  bottom: 265px;
  left: 37px;
  height: 6px;
  width: 40px;
  background: linear-gradient(
    270deg,
    #0edaa0ff,
    #30dc90ff,
    #51dd81ff,
    #73df71ff,
    #94e061ff
  );
}
.title-section::before {
  content: "";
  position: absolute;
  bottom: 265px;
  left: 20px;
  height: 6px;
  width: 10px;
  background: linear-gradient(
    270deg,
    #0edaa0ff,
    #30dc90ff,
    #51dd81ff,
    #73df71ff,
    #94e061ff
  );
}
#section-btn {
  margin-top: 80px;
}
</style>
