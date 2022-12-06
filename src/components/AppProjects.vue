<script>
import CardProject from "./CardProject.vue";
import AppSpacer from "./AppSpacer.vue";
import AppButton from "./AppButton.vue";

export default {
  components: {
    AppSpacer,
    CardProject,
    AppButton,
  },
  data() {
    return {
      projects: [
        {
          image: "src/assets/ina-soulis-227104-unsplash-1024x1024.jpg",
          description: "A famous Ferris Wheel",
          type: "marketing",
        },
        {
          image: "src/assets/sunisa-misa-531163-unsplash-1024x1024.jpg",
          description: "A famous Ferris Wheel",
          type: "marketing",
        },
        {
          image: "src/assets/355H-1024x1024.jpg",
          description: "A famous Ferris Wheel",
          type: "marketing",
        },
        {
          image: "src/assets/photo-1448932252197-d19750584e56-1024x1024.jpg",
          description: "A famous Ferris Wheel",
          type: "marketing",
        },
        {
          image: "src/assets/business-competition-PB366D8-1024x1024.jpg",
          description: "Business competition",
          type: "marketing",
        },
        {
          image: "src/assets/cozy-sofa-in-living-room-PQR5AB9-1024x1024.jpg",
          description: "Cozy sofa in living room",
          type: "marketing",
        },
        {
          image: "src/assets/aa9a4539-PQGJ7HU-1024x1024.jpg",
          description: "Online Marketing",
          type: "marketing",
        },
        {
          image: "src/assets/cody-davis-253928-unsplash-1024x1024.jpg",
          description: "Cody davis",
          type: "marketing",
        },
      ],
    };
  },
};
</script>
<template>
  <section>
    <div class="description d-flex">
      <div class="title">
        <AppSpacer />
        <h3>
          Our recent <mark>web designs</mark>& <br />
          some examples of <br />
          past projects
        </h3>
        <AppSpacer />
      </div>
      <div class="content">
        <p>
          Far far away, behind the word mountains, far from the countries
          Vokalia and Consonantia, there live the blind texts. Separated they
          live in Bookmarksgrove right at th3e coast of the Semantics, a large
          language ocean Separated tthey live in Bookmarksgrove. Far far away,
          behind the word mountains, far from the countries Vokalia and
          Consonantia, there live the blind texts. Separated they live in
          Bookmarksgrove right at th3e coast of the Semantics, a large language
          ocean Separated tthey live in Bookmarksgrove.
        </p>
      </div>
    </div>
    <div id="examples" class="d-flex flex-wrap my-5">
      <CardProject
        class="px-2 py-1"
        v-for="project in projects"
        :img="project.image"
        :description="project.description"
        :type="project.type"
      />
      <div id="settings">
        <div class="setting-btn">
          <span class="mx-2"
            ><i class="fa-solid fa-table-cells-large"></i
          ></span>
          <span>Browse Demos</span>
        </div>
        <div class="setting-btn">
          <span class="mx-2"><i class="fa-solid fa-bag-shopping"></i></span>
          <span>Buy Now!</span>
        </div>
        <div class="setting-btn">
          <span class="mx-2"><i class="fa-solid fa-file-export"></i></span>
          <span>Export Section</span>
        </div>
      </div>
    </div>
    <div id="btn">
      <AppButton />
    </div>
  </section>
</template>

<style lang="scss" scoped>
section {
  padding: 200px 0;
  #btn {
    text-align: center;
    margin-top: 80px;
  }
}
.title {
  width: 40%;
}
.content {
  width: 70%;
  align-self: flex-end;
}
h3 {
  margin: 30px 10px;
  font-size: 40px;
  font-weight: bold;
  mark {
    background-color: inherit;
    color: var(--tertiary-color);
  }
}
#examples {
  position: relative;
  #settings {
    position: absolute;
    right: 0;
    top: 200px;
  }
  .setting-btn {
    background-color: rgba($color: #000000, $alpha: 0.5);
    color: white;
    padding: 10px;
    font-size: 14px;
    margin-bottom: 10px;
    border-radius: 10px 0 0 10px;
    i {
      font-size: 18px;
    }
  }
}
</style>
