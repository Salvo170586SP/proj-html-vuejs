<template>
  <div id="footer-top" class="text-white">
    <div class="container">
      <div class="row">
        <div class="col-3">
          <img src="../assets/images/white-logo-2.png" alt="logo" />
          <p class="my-5 c-green">
            When, while the lovely valley teems vapour aroundmeand meridian sun
            strikes the upper impenetrable
          </p>
        </div>
        <div class="col-3 px-5">
          <h5>Quick links</h5>
          <ul class="p-0">
            <li v-for="(link, id) in links" :key="id">
              <a href="#">{{ link.text }}</a>
            </li>
          </ul>
        </div>
        <div class="col-3 px-5 text-center">
          <h5 class="mb-4" >Resources</h5>
          <ul class="p-0 m-left" >
            <li v-for="(resource, id) in resources" :key="id">
              <a href="#">{{ resource.text }}</a>
            </li>
          </ul>
        </div>
        <div class="col-3">
          <h5>Contact Us</h5>
          <address class="py-4 c-green">
            <strong class="text-white">Address :</strong> C.Amedee 4401 Waldeck
            <br />
            Street Grapevine Nashville, Tx 76051
          </address>
          <p class="c-green">
            <strong class="text-white">Phone:</strong> +99(0) 101 0000 888
          </p>
          <p class="c-green">
            <strong class="text-white">Email:</strong> Info@yourdomain.com
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "FooterTop",
  props: ["links", "resources"],
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";

#footer-top {
  height: 400px;
  background-color: $bg-blue;

  .m-left{
    margin-left: 100px;
  }

  li {
    line-height: 35px;
  }
  
  a,
  .c-green {
    color: $paragraph-color;
  }
}
</style>