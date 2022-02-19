<template>
   <div id="footer-bottom" class="text-white">
        <div class="container">
          <div class="row">
            <div
              class="col-12 d-flex justify-content-between align-items-center"
            >
              <p>@2020 Phlox.All Rights Reserved</p>

              <div class="social">
                <i class="fa-brands fa-instagram"></i>
                <i class="fa-brands fa-linkedin-in"></i>
                <i class="fa-brands fa-facebook-f"></i>
                <i class="fa-brands fa-twitter"></i>
              </div>
            </div>
          </div>
        </div>
      </div>
</template>

<script>
export default {
    name: 'FooterBottom',
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";


#footer-bottom {
  height: 80px;
  background-color: $bg-blue;
}

p {
  color: $paragraph-color;
}

i {
  margin-left: 20px;
}
</style>