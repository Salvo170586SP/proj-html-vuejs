<template>
  <div id="app">
    <Header />
    <main>
      <section id="services">
        <div class="container">
          <div class="row">
            <div class="col-12 text-center">Our Services</div>
            <div class="col-12 text-center">What We Do</div>
            <div class="col-12 text-center">When wile the lovely valley teems whit vapour around meand the</div>
          </div>
          <div class="row">
            <div class="col-3">item</div>
            <div class="col-3">item</div>
            <div class="col-3">item</div>
            <div class="col-3">item</div>
          </div>
        </div>
      </section>
    </main>
  </div>
</template>

<script>
import Header from "./components/Header.vue";

export default {
  name: "App",
  components: { Header },
  data(){
    return{
      headerItems: [
       { url:'#', text:'contatti'},
       { url:'#', text:'home'},
       { url:'#', text:'gallery'}
      ]
    }
  }
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
li{
  list-style-type: none;
}

a{
  color: white;
  text-decoration: none;
}

  /* HEADER */
  header{
    background-color: #527CEB;
  }
</style>
