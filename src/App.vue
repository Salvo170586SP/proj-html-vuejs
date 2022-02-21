<template>
  <div id="app">
    <header id="header">
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
      <a href="#header"><i class="fa-solid fa-arrow-up"></i></a>     
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
    FooterBottom,
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

/* HEADER */
header {
  background-color: $bg-blue;
  height: 100vh;
}

footer{
    background-color: $bg-blue;
}

.fa-arrow-up{
  background-color: white;
  padding: 15px;
  border-radius: 50%;
  border: 1px solid $bg-blue;
  position: fixed;
  bottom: 50px;
  right: 50px;
  color: $bg-blue;
  cursor: pointer;
}

</style>
