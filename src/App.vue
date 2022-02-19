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
            <div class="col-3">
              <img src="./assets/images/white-logo-2.png" alt="logo" />
              <p class="my-5 c-green">
                When, while the lovely valley teems vapour aroundmeand 
                meridian sun strikes the upper impenetrable
              </p>
            </div>
            <div class="col-3 px-5">
              <h5>Quick links</h5>
              <ul class="p-0">
                <li><a href="#">Services</a></li>
                <li><a href="#">Contact</a></li>
                <li><a href="#">Blog</a></li>
              </ul>
            </div>
            <div class="col-3 px-5">
              <h5>Resources</h5>
              <ul class="p-0">
                <li><a href="#">Art Design</a></li>
                <li><a href="#">Computer</a></li>
                <li><a href="#">IT News</a></li>
                <li><a href="#">Networking</a></li>
                <li><a href="#">Web Security</a></li>
              </ul>
            </div>
            <div class="col-3">
              <h5>Contact Us</h5>
              <address class="py-4 c-green"><strong class="text-white">Address :</strong> C.Amedee 4401 Waldeck <br>
                Street Grapevine Nashville, Tx 76051
              </address>
              <p class="c-green"><strong class="text-white">Phone:</strong> +99(0) 101 0000 888 </p>
              <p class="c-green"><strong class="text-white">Email:</strong> Info@yourdomain.com</p>
            </div>
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
    SectionSubscribe,
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

#footer-top {
  height: 400px;
  background-color: $bg-blue;
}

.c-green{
  color: $paragraph-color;
}
</style>
