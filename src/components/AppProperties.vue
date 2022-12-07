<script>
import CardProperties from "./commons/CardProperties.vue";
import AppButton from "./commons/AppButton.vue";
import AppSpacer from "./commons/AppSpacer.vue";

export default {
  components: {
    CardProperties,
    AppButton,
    AppSpacer,
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
      <AppSpacer class="spacer" />
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
.spacer {
  padding-top: 30px;
}
.card-section {
  display: flex;
  flex-wrap: wrap;
  width: 65%;
  justify-content: space-around;
}

#section-btn {
  margin-top: 60px;
}
</style>
