<script>
import AppSpacer from "./commons/AppSpacer.vue";

export default {
  components: {
    AppSpacer,
  },
  data() {
    return {
      quicklinks: [
        "Careers",
        "News",
        "Terms of use",
        "Privacy Projects",
        "About",
        "Contact",
      ],
    };
  },
};
</script>

<template>
  <footer>
    <div class="d-flex justify-content-between">
      <div class="company-story my-col">
        <img class="mb-3" src="../assets/cropped-Group-39-2x.png" alt="" />
        <p>
          While the lovely valley teems with vapour around me, and the meridian
          sun strikes the upper surface of the impenetrable foliage of mu trees.
          While the lovely valley teems with vapour around me.
        </p>
      </div>
      <div class="quick-links my-col">
        <h4>QUICK LINKS</h4>
        <AppSpacer class="spacer" />
        <ul>
          <li v-for="quicklink in quicklinks">
            <a href="#">{{ quicklink }}</a>
          </li>
        </ul>
      </div>
      <div class="contact my-col">
        <h4>CONTACT</h4>
        <AppSpacer class="spacer" />
        <ul>
          <li class="pb-4">
            Patricia C. Amedee 4401 Waldeck Street Grapevine Nashville, TX 76051
          </li>
          <li class="pb-4">info@yourdomain.com</li>
          <li class="pb-4">+99 (0) 101 000 888</li>
        </ul>
      </div>
      <div class="location my-col">
        <h4>LOCATION ON MAP</h4>
        <AppSpacer class="spacer" />
        <img src="../assets/map.png" alt="" />
      </div>
    </div>
    <div class="copyright d-flex justify-content-between">
      <div>
        <i class="fa-regular fa-copyright me-2"></i>
        <small>2020 PHLOX BUSINESS THEME.</small>
      </div>
      <div class="social-links">
        <i class="fa-brands fa-facebook-f"></i>
        <i class="fa-brands fa-twitter px-3"></i>
        <i class="fa-brands fa-pinterest-p"></i>
      </div>
    </div>
  </footer>
  <div class="chat-section">
    <div id="up">
      <i class="fa-solid fa-arrow-up"></i>
    </div>
    <div id="chat">
      <i class="fa-regular fa-comment"></i>
    </div>
  </div>
</template>

<style lang="scss" scoped>
footer {
  background-color: white;
  padding-top: 100px;
}
.my-col {
  width: calc(100% / 4);
  padding: 0 20px 150px 20px;
  .spacer {
    padding: 10px 0 30px 0;
  }
  h4 {
    font-weight: bold;
  }
}
ul {
  list-style: none;
  padding-left: 0;
  a {
    text-decoration: none;
    color: inherit;
  }
}
.location > img {
  width: 100%;
}
.copyright {
  background: linear-gradient(270deg, black, rgb(48, 48, 48));
  color: grey;
  padding: 40px 20px;
}
.chat-section {
  display: flex;
  position: fixed;
  bottom: 0;
  right: 200px;
  left: 0;
  z-index: 40;
  background-color: transparent;
  justify-content: flex-end;
  padding-bottom: 50px;
  height: 100px;
  align-items: center;
}
#chat {
  margin-left: 20px;
  width: 50px;
  height: 50px;
  background-color: #527ceb;
  color: white;
  border: none;
  border-radius: 50%;
  font-size: 20px;
  text-align: center;
  line-height: 50px;
}
#up {
  background-color: white;
  border: 1px solid black;
  border-radius: 50%;
  width: 30px;
  height: 30px;
  text-align: center;
  line-height: 30px;
}
</style>
