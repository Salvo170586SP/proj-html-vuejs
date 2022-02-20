<template>
  <section id="your-project" class="d-flex align-items-center">
    <div class="container">
      <!-- image section -->
      <div class="row">
        <div class="col-6">
          <figure>
            <img src="../assets/images/men-data.png" alt="men data" />
          </figure>
        </div>
        <div class="col-6">
          <!-- text section -->
          <div class="row">
            <div class="col-12 text-white">Start Your Project</div>
            <div class="col-12 title-section">Grow Your Business</div>
            <div class="col-12 subtitle-section">With Our Strategy</div>
            <div class="col-12 py-4">
              <p>
                When, while the lovely valley teems with vapour around meand the
                meridian sun strikes the upper surface. of the impenetrable
                foliage of my trees and but a few stray gleams steal into the
                inner sanctuary
              </p>
            </div>
            <div class="col-12">
              <a href="#" class="red-btn">Try It Now</a>
              <a href="#" class="blue-btn">Explore More</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "SectionProject",
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";

#your-project {
  background-color: $bg-blue;
  height: 700px;

  figure {
    width: 400px;
    img {
      width: 100%;
    }
  }

  .title-section {
    font-size: 4rem;
    font-weight: bold;
    color: white;
  }

  .subtitle-section {
    font-size: 4rem;
    color: white;
  }

  a {
    border-radius: 25px;
    padding: 10px 30px;
    background-color: $btn-blue;
    margin-right: 10px;
    &.blue-btn {
      background: rgb(2, 0, 36);
      background: linear-gradient(
        270deg,
        rgba(2, 0, 36, 1) 0%,
        rgba(36, 36, 115, 1) 0%,
        rgba(0, 160, 186, 1) 100%
      );
    }
    &.red-btn {
      background: rgb(0, 29, 36);
      background: linear-gradient(
        90deg,
        rgba(0, 29, 36, 1) 0%,
        rgba(100, 133, 145, 1) 0%,
        rgba(227, 18, 47, 1) 100%
      );
    }
  }

  p {
    color: $paragraph-color;
  }
}
</style>