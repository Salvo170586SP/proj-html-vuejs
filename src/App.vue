<template>
  <div id="app">
    <Header :items="headerItems" />
    <main>
      <SectionServices />
      <SectionProject />
      <SectionPortfolio />
      <SectionPrice />
      <SectionBlog />
      <SectionTestimonial />
      <SectionSubscribe />
    </main>
    <footer>
      <div id="footer-top" class="text-white">
        <div class="container">
          <div class="row">
            <div class="col-3">item</div>
            <div class="col-3">item</div>
            <div class="col-3">item</div>
            <div class="col-3">item</div>
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import SectionServices from "./components/SectionServices.vue";
import SectionProject from "./components/SectionProject.vue";
import SectionPortfolio from "./components/SectionPortfolio.vue";
import SectionPrice from "./components/SectionPrice.vue";
import SectionBlog from "./components/SectionBlog.vue";
import SectionTestimonial from "./components/SectionTestimonial.vue";
import SectionSubscribe from "./components/SectionSubscribe.vue";

export default {
  name: "App",
  components: {
    Header,
    SectionServices,
    SectionProject,
    SectionPortfolio,
    SectionPrice,
    SectionBlog,
    SectionTestimonial,
    SectionSubscribe
  },
  data() {
    return {
      headerItems: [
        { url: "#", text: "Home", active: true },
        { url: "#", text: "About", active: false },
        { url: "#", text: "Services", active: false },
        { url: "#", text: "Blog", active: false },
        { url: "#", text: "Contact", active: false },
        { url: "#", text: "Portfolio", active: false },
      ],
    };
  },
};
</script>



<style lang="scss">
@import "./assets/scss/style.scss";

/* da eliminare */
[class^="col"] {
  border: 1px solid red;
}
.container {
  border: 1px dotted blue;
}
/* da eliminare  */

#footer-top{
  height: 400px;
  background-color: $bg-blue;
}

</style>
