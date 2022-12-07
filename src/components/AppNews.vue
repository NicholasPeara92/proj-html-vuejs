<script>
import NewsCard from "./commons/NewsCard.vue";
import AppSpacer from "./commons/AppSpacer.vue";
import DarkButton from "./commons/DarkButton.vue";

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
      partners: [
        {
          img: "src/assets/client-1-2x.png",
          name: "Avantgarde",
        },
        {
          img: "src/assets/client-9-2x.png",
          name: "Fastlane",
        },
        {
          img: "src/assets/client-7-2x.png",
          name: "Ron Jones",
        },
        {
          img: "src/assets/client-3-2x.png",
          name: "Chippy's",
        },
        {
          img: "src/assets/client-4-2x.png",
          name: "Bullseye",
        },
        {
          img: "src/assets/client-5-2x.png",
          name: "Mighty Furnitures",
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
    <div id="start-choice" class="d-flex">
      <div class="card-left mx-3">
        <small>Are You Ready</small>
        <h4>Start a New project</h4>
        <form action="submit">
          <input
            type="email"
            class="l"
            id="exampleFormControlInput1"
            placeholder="Enter Your Email Adress"
          />
          <button id="submit" type="submit">SUBMIT</button>
        </form>
      </div>
      <div class="card-right mx-3">
        <small>What Are You Waiting For?</small>
        <h4>Let's Talk About Work</h4>
        <DarkButton />
      </div>
    </div>
    <div id="partners" class="d-flex">
      <div v-for="partner in partners">
        <img :src="partner.img" alt="" />
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
section {
  background-color: var(--secondary-color);
  padding-top: 200px;
  padding-bottom: 100px;
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
#start-choice {
  justify-content: space-between;
  padding-bottom: 100px;
  .card-left {
    background: linear-gradient(270deg, black, rgb(48, 48, 48));
    width: 50%;
    border-radius: 20px;
    box-shadow: 5px 5px 20px rgb(168 168 168);
  }
  .card-right {
    width: 50%;
    background: linear-gradient(
      270deg,
      #0edaa0ff,
      #30dc90ff,
      #51dd81ff,
      #73df71ff,
      #94e061ff
    );
    box-shadow: 5px 5px 15px #baf5e7;
    border-radius: 20px;
  }
}
.card-left,
.card-right {
  color: white;
  text-align: center;
  padding: 50px 0;
  h4 {
    margin-top: 20px;
    margin-bottom: 50px;
    font-weight: bold;
  }
  small {
    color: lightgray;
  }
}
input,
#submit {
  color: grey;
  background-color: var(--primary-color);
  border: none;
  padding: 10px 20px;
  font-size: 14px;
}
input {
  border-radius: 20px 0 0 20px;
}
#submit {
  border-radius: 0 20px 20px 0;
}
#partners {
  justify-content: space-between;
  align-items: center;
  padding: 30px;
}
</style>
