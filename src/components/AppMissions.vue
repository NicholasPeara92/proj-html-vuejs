<script>
import AppButton from "./commons/AppButton.vue";
import AppSpacer from "./commons/AppSpacer.vue";

export default {
  components: {
    AppButton,
    AppSpacer,
  },
};
</script>

<template>
  <section class="d-flex">
    <div class="img-col">
      <div class="img-back">
        <img src="../assets/busy-architect-PYVKWM4-1024x872.jpg" alt="" />
        <div id="veil"></div>
      </div>
      <div class="img-front">
        <img
          src="../assets/businesswoman-analysing-document-P8WSNMC-1024x820.jpg"
          alt=""
        />
      </div>
    </div>
    <div class="description-col">
      <h3>
        learn more about <br />
        our<mark>missions</mark>
      </h3>
      <AppSpacer class="spacer" />
      <p>
        Far far away, behind the word mountains, far from the countries Vokalia
        and Consonantia, there live the blind texts. Separated they live in
        Bookmarksgrove right at th3e coast of the Semantics, a large language
        ocean Separated tthey live in Bookmarksgrove.
      </p>
      <AppButton />
    </div>
  </section>
</template>

<style lang="scss" scoped>
section {
  background-color: var(--secondary-color);
  justify-content: space-between;
  padding: 150px 0 200px 0;
}
.img-col {
  width: 50%;
  position: relative;
}
.description-col {
  width: 50%;
  padding: 100px;
  h3 {
    font-size: 42px;
    font-weight: bold;
  }
  p {
    margin-top: 30px;
    margin-bottom: 30px;
  }
  mark {
    background-color: inherit;
    color: var(--tertiary-color);
  }
}
.spacer {
  padding-top: 15px;
}

.img-back {
  max-width: 620px;
  position: relative;
  #veil {
    position: absolute;
    top: 0;
    bottom: 0;
    right: 0;
    left: 0;
    background: linear-gradient(
      270deg,
      #0edaa0ff,
      #30dc90ff,
      #51dd81ff,
      #73df71ff,
      #94e061ff
    );
    border-radius: 0 20px 20px 0;
    opacity: calc(0.8);
  }
  img {
    border-radius: 20px;
    width: 100%;
  }
}
.img-front {
  max-width: 650px;
  position: absolute;
  top: 50px;
  left: 100px;
  img {
    width: 100%;
    border-radius: 10px;
    box-shadow: 5px 5px 20px rgb(168, 168, 168);
  }
}
</style>
