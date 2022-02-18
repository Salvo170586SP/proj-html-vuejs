<template>
  <header class="py-3">
    <div class="container text-white">
      <!-- header-top -->
      <div id="header-top" class="row align-items-center">
        <div class="col-3">
          <img src="../assets/images/white-logo-2.png" alt="logo" />
        </div>
        <div class="col-8">
          <nav class="d-flex justify-content-end">
            <ul v-for="(item, index) in items" :key="index" class="p-0">
              <li><a href="#">{{ item.text }}</a></li>
            </ul>
          </nav>
        </div>
        <div class="col-1">
          <a class="sing-in-btn" href="#">Sing-in</a>
        </div>
      </div>

      <!-- header-bottom/spotlyght -->
      <div id="header-bottom" class="row align-items-center">
        <div class="col-4 pt-5">
          <h1 class="fs-1 mb-3">
            Business Planning
            <span>Digital Tecnoogy</span>
            Modern Solution!
          </h1>
          <p class="mb-5">
            When, while the lovely valley teems with vapour around meand the
            meridian sun strikes the upper surface.
          </p>

          <a href="#" class="try-btn px-4 mx-3">Try It Now</a>
          <a href="#" class="explore-btn px-4">Explore More</a>
        </div>

        <div class="col-8 px-5">
            <img src="../assets/images/header.png" alt="header-img" />
        </div>
      </div>
    </div>
  </header>
</template>

<script scoped>
export default {
  name: "Header",
  props: ["items"],
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";

/* link button */
a {
  border-radius: 25px;
  padding: 10px;
}

.sing-in-btn,
.try-btn,
.explore-btn {
  background-color: $btn-blue;
}


/* text */
h1 {
  margin-top: 50px;
}

span{
    font-weight: 400;
}

p{
 color: $paragraph-header;
}

/* HEADER */
header {
  background-color: $header-bg;
}
</style>