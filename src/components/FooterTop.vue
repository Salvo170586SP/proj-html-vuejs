<template>
  <div id="footer-top" class="text-white">
        <div class="container">
          <div class="row">
            <div class="col-3">
              <img src="../assets/images/white-logo-2.png" alt="logo" />
              <p class="my-5 c-green">
                When, while the lovely valley teems vapour aroundmeand 
                meridian sun strikes the upper impenetrable
              </p>
            </div>
            <div class="col-3 px-5">
              <h5>Quick links</h5>
              <ul class="p-0" v-for="(link, id) in links" :key="id">
                <li><a href="#">{{link.text}}</a></li>
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
</template>

<script>
export default {
    name: 'FooterTop',
    props:['links']
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";

#footer-top {
  height: 400px;
  background-color: $bg-blue;
}

li{
    line-height: 30px;
}

a, .c-green{
  color: $paragraph-color;
}

 
</style>