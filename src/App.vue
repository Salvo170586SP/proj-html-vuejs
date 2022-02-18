<template>
  <div id="app">
    <Header :items="headerItems" />
    <main>
      <SectionServices />
      <SectionProject />
    </main>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import SectionServices from "./components/SectionServices.vue";
import SectionProject from "./components/SectionProject.vue";

export default {
  name: "App",
  components: { Header, SectionServices, SectionProject },
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


</style>
