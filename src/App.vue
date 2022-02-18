<template>
  <div id="app">
    <Header :items="headerItems"  />
    <main>
      <SectionServices />
      <section id="your-project">
        <div class="container">
          <div class="row">
            <div class="col-6">IMG</div>
            <div class="col-6">TEXT</div>
          </div>
        </div>
      </section>
    </main>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import SectionServices from "./components/SectionServices.vue";

export default {
  name: "App",
  components: { Header, SectionServices },
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

#your-project{
  background-color: $bg-blue;
}


</style>
