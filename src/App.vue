<template>
  <div id="app">
    <Header />
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
