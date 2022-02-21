<template>
  <section id="portfolio">
    <div class="container">
      <div class="row">
        <div class="col-6 py-5">
          <span>Portfolio</span>
          <h2><strong>lastest</strong> work</h2>
        </div>
        <div class="col-6 d-flex align-items-center justify-content-end">
          <i class="fa-solid fa-arrow-left-long"></i>
          <i class="fa-solid fa-arrow-right-long"></i>
        </div>
      </div>

      <!-- cards portfolio -->
      <div class="row">
        <div class="col-4">
          
          <!-- card -->
          <div class="card bg-red">
            <figure>
              <img
                class="img-fluid"
                src="../assets/images/8wa60okr-1-790x576.jpg"
                alt=""
              />
            </figure>
            <div class="row py-2">
              <div class="col-7 fw-bold">Bascket of flower on table</div>
              <div class="col-5">Branding Strategy</div>
            </div>
          </div>
        </div>

        <div class="col-4">
          <!-- card -->
          <div class="card bg-red">
            <figure>
              <img
                class="img-fluid"
                src="../assets/images/DRY-1-790x576.jpg"
                alt=""
              />
            </figure>
            <div class="row py-2">
              <div class="col-7 fw-bold">Purinky Products</div>
              <div class="col-5">Digital Experience</div>
            </div>
          </div>
        </div>

        <div class="col-4">
          <!-- card -->
          <div class="card bg-red">
            <figure>
              <img
                class="img-fluid"
                src="../assets/images/a247b00b-3621-470f-b4b8-b3ac46f25907-1-790x576.jpg"
                alt=""
              />
            </figure>
            <div class="row py-2">
              <div class="col-7 fw-bold">Satisfy Poster</div>
              <div class="col-5">Branding Strategy</div>
            </div>
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

#portfolio{
  height: 100vh;
  display: flex;
  align-items: center;
}

span {
  color: $red-span;
}

i {
  color: $red-span;
  cursor: pointer;
  border: 1px solid $red-span;
  margin-right: 15px;
  border-radius: 50%;
  padding: 15px;
}

.card {
  border-radius: 20px;
  text-align: center;
  cursor: pointer;
  border: 0;

  &:hover.bg-red {
    background: linear-gradient(
      90deg,
      rgba(0, 29, 36, 1) 0%,
      rgba(100, 133, 145, 1) 0%,
      rgba(227, 18, 47, 1) 100%
    );
    color: white;
  }
}

figure {
  overflow: hidden;
  border-radius: 20px;
}

.dot-img {
  width: 10px;
  height: 10px;
  background-color: $red-span;
  border-radius: 50%;
  margin-right: 20px;
}
</style>