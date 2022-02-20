<template>
  <section id="services" class="d-flex align-items-center">
    <div class="container">
      <div class="row py-5">
        <div class="col-12 text-center"><span>Our Services</span></div>
        <div class="col-12 h2 text-center"><strong>What</strong> We Do</div>
        <div class="col-12 text-center">
          When wile the lovely valley teems whit vapour around meand the
        </div>
      </div>

      <!-- card services -->
      <div class="row text-center align-items-end card-services">
        <div class="col-3">
          <div class="row">
            <div class="col-12 d-flex justify-content-center">
              <figure>
                <img src="../assets/images/Group-247.png" alt="data analysis" />
              </figure>
            </div>
            <div class="col-12 h3">Data Analysis</div>
            <div class="col-12">
              <p>
                When, while the lovely valley teems with vapour around meand the
                meridian sun strikes the upper
              </p>
            </div>
          </div>
        </div>
        <div class="col-3">
          <div class="row">
            <div class="col-12 d-flex justify-content-center">
              <figure>
                <img src="../assets/images/Group-567.png" alt="" />
              </figure>
            </div>
            <div class="col-12 h3">Seo Optimization</div>
            <div class="col-12">
              <p>
                When, while the lovely valley teems with vapour around meand the
                meridian sun strikes the upper
              </p>
            </div>
          </div>
        </div>
        <div class="col-3">
          <div class="row">
            <div class="col-12 d-flex justify-content-center">
              <figure>
                <img src="../assets/images/Group-538.png" alt="" />
              </figure>
            </div>
            <div class="col-12 h3">Security Data</div>
            <div class="col-12">
              <p>
                When, while the lovely valley teems with vapour around meand the
                meridian sun strikes the upper
              </p>
            </div>
          </div>
        </div>
        <div class="col-3">
          <div class="row">
            <div class="col-12 d-flex justify-content-center">
              <figure>
                <img src="../assets/images/Group-566.png" alt="" />
              </figure>
            </div>
            <div class="col-12 h3">Branding strategy</div>
            <div class="col-12">
              <p>
                When, while the lovely valley teems with vapour around meand the
                meridian sun strikes the upper
              </p>
            </div>
          </div>
        </div>
      </div>
      <div class="row">
        <div class="col-12 text-center">
          <a href="#">View All Services</a>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "SectionServices",
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";

#services {
  height: 850px;
}

/* utility */
a {
  border-radius: 25px;
  padding: 10px 15px;
  background: rgb(0, 29, 36);
  background: linear-gradient(
    90deg,
    rgba(0, 29, 36, 1) 0%,
    rgba(100, 133, 145, 1) 0%,
    rgba(227, 18, 47, 1) 100%
  );
}

span {
  color: $red-span;
}

figure {
  width: 150px;
}

img {
  width: 100%;
}

/* CARD-SERVICES */

.card-services {
  margin-bottom: 200px;
}
</style>