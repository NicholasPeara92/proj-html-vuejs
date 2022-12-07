<script>
import DarkButton from "./commons/DarkButton.vue";
import AppSpacer from "./commons/AppSpacer.vue";

export default {
  components: {
    DarkButton,
    AppSpacer,
  },
};
</script>

<template>
  <div class="background">
    <div class="hero">
      <div id="description">
        <small>17 YEARS OF EXPERIENCE</small>
        <h1>
          We Are a <br />
          Web Design<mark>Agency</mark>
        </h1>
        <AppSpacer class="spacer" />
        <p class="pt-5">
          Far ffar away, behind the word mountains , far from the countries
          Vokalia and Consonantia, there live the blind texts. Separated they
          live in Bookmarksgrove right at the coast of the Semantics, a large
          language ocean. Separated they live in Bookmarksgrove.
        </p>
        <DarkButton class="mt-4" />
        <div class="d-flex justify-content-between align-items-center pt-5">
          <ul>
            <li><a href="#">FACEBOOK</a></li>
            <li>- <a href="#">INSTAGRAM</a></li>
            <li>- <a href="#">YOUTUBE</a></li>
            <li>- <a href="#">TWITTER</a></li>
          </ul>
          <div class="btn-group">
            <a href="#" class="btn active" aria-current="page">01</a>
            <a href="#" class="btn">02</a>
            <a href="#" class="btn">03</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.background {
  background-color: var(--secondary-color);
}
.hero {
  background-image: url(../assets/Group-36-2x.png);
  background-size: contain;
  background-position: 650px -48px;
  background-repeat: no-repeat;
  height: 935px;
}
#description {
  max-width: 750px;
  padding-left: 120px;
  padding-top: 140px;
  h1 {
    font-size: 58px;
    font-weight: bold;
    line-height: 70px;
  }
  .spacer {
    margin: 30px 0;
  }
}
small {
  color: var(--tertiary-color);
  letter-spacing: 5px;
}
mark {
  background-color: inherit;
  color: var(--tertiary-color);
}
ul {
  list-style: none;
  display: flex;
  padding-left: 0;
  align-items: center;
  margin-bottom: 0;
  li {
    margin-right: 5px;
  }
  a {
    color: inherit;
    text-decoration: none;
    font-weight: bold;
  }
}
.btn-group {
  background-color: var(--primary-color);
  border: 2px solid var(--primary-color);
  border-radius: 20px;
  a {
    color: white;
  }
}
.active {
  border-radius: 20px;
  border: none;
  background: linear-gradient(
    270deg,
    #0edaa0ff,
    #30dc90ff,
    #51dd81ff,
    #73df71ff,
    #94e061ff
  );
}
</style>
