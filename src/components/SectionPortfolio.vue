<template>
  <section id="portfolio">
    <div class="container">
      <div class="row">
        <div class="col-6 py-5">
          <span>Portfolio</span>
          <h2><strong>lastest</strong> work</h2>
        </div>
        <div class="col-6 d-flex align-items-center justify-content-end">
          <i @click="prevPic" class="fa-solid fa-arrow-left-long"></i>
          <i @click="nextPic" class="fa-solid fa-arrow-right-long"></i>
        </div>
      </div>
    </div>

    <!-- cards portfolio -->
    <div class="container-fluid">
      <div class="row">
        <div class="col-12 d-flex overflow">

          <!-- card -->
          <div
            class="card bg-red mx-1"
            v-for="(card, index) in slidersCards"
            :key="index"
            :class="{ opacity: cardActive(index) }"
          >
            <figure>
              <img class="img-fluid" :src="card.url" alt="" />
            </figure>
            <div class="row py-2">
              <div class="col-7 fw-bold">{{ card.title }}</div>
              <div class="col-5">{{ card.subtitle }}</div>
            </div>
          </div>
        </div>
      </div>

      <div class="row">
        <div class="col-12 p-5 d-flex justify-content-center">

          <!-- dot-img -->
          <div
            v-for="(card, index) in slidersCards"
            :key="index"
            class="dot-img"
            :class="{ active: dotActive(index) }"
          ></div>
          
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "SectionPortfolio",
  data() {
    return {
      currentIndex: 0,
      slidersCards: [
        {
          url: require("../assets/images/8wa60okr-1-790x576.jpg"),
          title: "Bascket of flower on table",
          subtitle: "Branding Strategy",
        },
        {
          url: require("../assets/images/DRY-1-790x576.jpg"),
          title: "Purinky Products",
          subtitle: "Digital Experience",
        },
        {
          url: require("../assets/images/a247b00b-3621-470f-b4b8-b3ac46f25907-1-790x576.jpg"),
          title: "Satisfy Poster",
          subtitle: "Branding Strategy",
        },
        {
          url: require("../assets/images/84316050-0af0-49db-a53a-241d47ddad0e-2-790x576.jpg"),
          title: "Satisfy Poster",
          subtitle: "Branding Strategy",
        },
      ],
    };
  },
  methods: {
    prevPic() {
      if (this.currentIndex === 0) {
        this.currentIndex = this.slidersCards.length - 1;
      } else {
        this.currentIndex--;
      }
    },
    nextPic() {
      if (this.currentIndex === this.slidersCards.length - 1) {
        this.currentIndex = 0;
      } else {
        this.currentIndex++;
      }
    },
    dotActive(index) {
      return this.currentIndex === index;
    },
    cardActive(index) {
      return this.currentIndex !== index;
    },
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";

#portfolio {
  height: 100vh;
  display: flex;
  justify-content: center;
  flex-direction: column;
}

span {
  color: $red-span;
}

i {
  color: $red-span;
  cursor: pointer;
  border: 1px solid $red-span;
  margin-right: 15px;
  border-radius: 50%;
  padding: 15px;
}

.card {
  border-radius: 20px;
  text-align: center;
  cursor: pointer;
  border: 0;
  min-width: 450px;
  &.opacity {
    opacity: 0.7;
  }

  &:hover.bg-red {
    background: linear-gradient(
      90deg,
      rgba(0, 29, 36, 1) 0%,
      rgba(100, 133, 145, 1) 0%,
      rgba(227, 18, 47, 1) 100%
    );
    color: white;
  }
}

.overflow {
  overflow: hidden;
}

figure {
  overflow: hidden;
  border-radius: 20px;
}

.dot-img {
  width: 10px;
  height: 10px;
  border: 1px solid $red-span;
  border-radius: 50%;
  margin-right: 20px;

  &.active {
    background-color: $red-span;
  }
}
</style>