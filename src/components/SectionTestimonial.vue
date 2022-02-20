<template>
  <section id="testimonial">
    <div class="container">
      <div class="row">
        <div class="col-12 text-center">
          <span class="red-span">Testimonial</span>
          <h2><strong>What</strong> Peolple Say</h2>
          <p>
            When, while the lovely valley teems with vapour around meand the
            meridian sun strikes the upper surface.
          </p>
        </div>
      </div>
      <div class="row">
        <div class="col-4">
          <!-- card testimonial -->
          <div
            class="card-testimonial py-5 d-flex flex-column align-items-center"
          >
            <div class="img-card">
              <figure>
                <img
                  class="img-fluid"
                  src="../assets/images/szabo-viktor-1266895-unsplash-1024x1024.png"
                  alt=""
                />
              </figure>
              <div class="vote py-4">
                <i class="fa-solid fa-star"></i>
                <i class="fa-solid fa-star"></i>
                <i class="fa-solid fa-star"></i>
                <i class="fa-regular fa-star"></i>
                <i class="fa-regular fa-star"></i>
              </div>
            </div>
            <div class="text-card text-center">
              <p>
                When, while the lovely valley teems with vapour around meand the
                meridian sun strikes the upper surface. of the impenetrable
                foliage of my trees and but a thousand
              </p>
              <h6>Michkel Anegl</h6>
              <p>Marketing Management</p>
            </div>
          </div>
        </div>
        <div class="col-4">
          <!-- card testimonial -->
          <div
            class="card-testimonial py-5 d-flex flex-column align-items-center"
          >
            <div class="img-card">
              <figure>
                <img
                  class="img-fluid"
                  src="../assets/images/philipe-cavalcante-539505-unsplash-1024x1024.png"
                  alt=""
                />
              </figure>
              <div class="vote py-4">
                <i class="fa-solid fa-star"></i>
                <i class="fa-solid fa-star"></i>
                <i class="fa-solid fa-star"></i>
                <i class="fa-regular fa-star"></i>
                <i class="fa-regular fa-star"></i>
              </div>
            </div>
            <div class="text-card text-center">
              <p>
                When, while the lovely valley teems with vapour around meand the
                meridian sun strikes the upper surface. of the impenetrable
                foliage of my trees and but a thousand
              </p>
              <h6>Michkel Anegl</h6>
              <p>Marketing Management</p>
            </div>
          </div>
        </div>
        <div class="col-4">
          <!-- card testimonial -->
          <div
            class="card-testimonial py-5 d-flex flex-column align-items-center"
          >
            <div class="img-card">
              <figure>
                <img
                  class="img-fluid"
                  src="../assets/images/fabio-spinelli-695744-unsplash-1024x1024.png"
                  alt=""
                />
              </figure>
              <div class="vote py-4">
                <i class="fa-solid fa-star"></i>
                <i class="fa-solid fa-star"></i>
                <i class="fa-solid fa-star"></i>
                <i class="fa-regular fa-star"></i>
                <i class="fa-regular fa-star"></i>
              </div>
            </div>
            <div class="text-card text-center">
              <p>
                When, while the lovely valley teems with vapour around meand the
                meridian sun strikes the upper surface. of the impenetrable
                foliage of my trees and but a thousand
              </p>
              <h6>Michkel Anegl</h6>
              <p>Marketing Management</p>
            </div>
          </div>
        </div>       
      </div>
      <div class="row">
          <div class="col-12 my-5  d-flex align-items-center justify-content-between">
            <img src="../assets/images/client-1-1.png" alt="golden logo" />
            <img src="../assets/images/clienty-2.png" alt="sweety logo" />
            <img src="../assets/images/clienty-4.png" alt="fastlane logo" />
            <img src="../assets/images/client-5.png" alt="mighty logo" />
            <img src="../assets/images/clienty-3.png" alt="jr logo" />
          </div>
        </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "SectionTestimonial",
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";

.red-span {
  color: $red-span;
}

figure {
  width: 100px;
  border-radius: 50%;
  overflow: hidden;
  box-shadow: 0 0 0 5px $brd-color;
}

.vote {
  color: $brd-color;
}
</style>