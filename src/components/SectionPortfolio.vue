<template>
  <section id="portfolio">
    <div class="container">
      <div class="row">
        <div class="col-6 py-5">
          <span>Portfolio</span>
          <h2><strong>lastest</strong> work</h2>
        </div>
        <div class="col-6"></div>
      </div>

      <!-- card portfolio -->
      <div class="row">
        <div class="col-4">
          <figure>
            <img
              class="img-fluid"
              src="../assets/images/DRY-1-790x576.jpg"
              alt=""
            />
          </figure>
          <div class="row">
            <div class="col-6 fw-bold">Purinky Products</div>
            <div class="col-6">Digital Experience</div>
          </div>
        </div>

        <div class="col-4">
          <figure>
            <img
              class="img-fluid"
              src="../assets/images/8wa60okr-1-790x576.jpg"
              alt=""
            />
          </figure>
          <div class="row">
            <div class="col-6 fw-bold">Basket of flower on table</div>
            <div class="col-6">Branding strategy</div>
          </div>
        </div>

        <div class="col-4">
          <figure>
            <img
              class="img-fluid"
              src="../assets/images/84316050-0af0-49db-a53a-241d47ddad0e-2-790x576.jpg"
              alt=""
            />
          </figure>
          <div class="row">
            <div class="col-6 fw-bold">Basket of flower on table</div>
            <div class="col-6">Branding strategy</div>
          </div>
        </div>       
      </div>

      <div class="row">
        <div class="col-12 p-5 d-flex justify-content-center">
          <div class="dot-img"></div>
          <div class="dot-img"></div>
          <div class="dot-img"></div>
          <div class="dot-img"></div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "SectionPortfolio",
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";
span {
  color: $red-span;
}

figure {
  border-radius: 20px;
  overflow: hidden;
}

.dot-img {
  width: 10px;
  height: 10px;
  background-color: $red-span;
  border-radius: 50%;
  margin-right: 20px;
}
</style>