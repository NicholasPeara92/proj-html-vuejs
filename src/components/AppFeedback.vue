<script>
export default {};
</script>

<template>
  <section>
    <div id="veil">
      <i class="fa-solid fa-quote-left"></i>
      <p>
        When it comes to barbequing, there are two main schools of <br />
        thought for the techniques that you can use. Freshly scrambled <br />
        eggs with applewood smoked bacon - are amazing!
      </p>
      <img
        src="../assets/businesswoman-analysing-document-P8WSNMC-1024x820.jpg"
        alt=""
      />
      <h5>LISSA DURBIN</h5>
      <small>Client</small>
    </div>
  </section>
</template>

<style lang="scss" scoped>
section {
  background-image: url(../assets/four-businesspeople-in-a-boardroom-with-paperwork-PC4V8H4.jpg);
  background-position: center;
  background-size: cover;
  background-repeat: no-repeat;
  height: 820px;
  text-align: center;
  position: relative;
  #veil {
    background-color: rgba($color: #373737, $alpha: 0.9);
    position: absolute;
    top: 0;
    bottom: 0;
    right: 0;
    left: 0;
    color: white;
    padding-top: 200px;
    p {
      font-style: italic;
      font-size: 24px;
      font-weight: lighter;
      margin: 40px 0;
    }
    i {
      font-size: 44px;
    }
    img {
      max-width: 80px;
      height: 80px;
      object-fit: cover;
      border-radius: 50%;
      border: 2px solid white;
      margin: 30px 0;
    }
  }
}
i,
h5 {
  color: var(--tertiary-color);
}
</style>
