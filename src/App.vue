<template>
  <div id="app">
    <header>
      <HeaderTop :items="headerItems" />
      <HeaderBottom />
    </header>
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
      <FooterTop :links="quickLinks" :resources="resourcesLinks" />
      <FooterBottom />
    </footer>
  </div>
</template>

<script>
import HeaderTop from "./components/HeaderTop.vue";
import HeaderBottom from "./components/HeaderBottom.vue";
import SectionServices from "./components/SectionServices.vue";
import SectionProject from "./components/SectionProject.vue";
import SectionPortfolio from "./components/SectionPortfolio.vue";
import SectionPrice from "./components/SectionPrice.vue";
import SectionBlog from "./components/SectionBlog.vue";
import SectionTestimonial from "./components/SectionTestimonial.vue";
import SectionSubscribe from "./components/SectionSubscribe.vue";
import FooterTop from "./components/FooterTop.vue";
import FooterBottom from "./components/FooterBottom.vue";

export default {
  name: "App",
  components: {
    HeaderTop,
    HeaderBottom,
    SectionServices,
    SectionProject,
    SectionPortfolio,
    SectionPrice,
    SectionBlog,
    SectionTestimonial,
    SectionSubscribe,
    FooterTop,
    FooterBottom
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

      quickLinks:[
        {url:'#', text: 'Services', active: false},
        {url:'#', text: 'Contact', active: false},
        {url:'#', text: 'Blog', active: false},
      ],

      resourcesLinks:[
        {url:'#', text: 'Art Design', active: false},
        {url:'#', text: 'Computer', active: false},
        {url:'#', text: 'IT News', active: false},
        {url:'#', text: 'Networking', active: false},
        {url:'#', text: 'Web Security', active: false},
      ]
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

/* HEADER */
header {
  background-color: $bg-blue;
  height: 900px;
}

</style>
