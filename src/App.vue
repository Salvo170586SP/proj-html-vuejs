<template>
  <div id="app">
    <Header :items="headerItems"  />
    <main>
      <SectionServices />
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

/* utility */
li {
  list-style-type: none;
}

a {
  color: white;
  text-decoration: none;
}

/* HEADER */
header {
  background-color: $header-bg;
}
</style>
