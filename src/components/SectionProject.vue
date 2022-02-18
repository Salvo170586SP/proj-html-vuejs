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
                <div class="col-12 title-section ">Grow Your Business</div>
                <div class="col-12 subtitle-section">With Our Strategy</div>
                <div class="col-12 py-4">
                  <p>
                    When, while the lovely valley teems with vapour around meand
                  the meridian sun strikes the upper surface. of the
                  impenetrable foliage of my trees and but a few stray gleams
                  steal into the inner sanctuary
                  </p>                 
                </div>
                <div class="col-12">
                  <a href="#">Try It Now</a>
                  <a href="#">Explore More</a>
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
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";

#your-project {
  background-color: $bg-blue;
  height: 700px;
}

figure {
  width: 400px;
}

img {
  width: 100%;
}

.title-section{
    font-size: 4rem;
    font-weight: bold;
    color: white;
}

.subtitle-section{
    font-size: 4rem;
    color: white;
}

a {
  border-radius: 25px;
  padding: 10px 30px;
  background-color: $btn-blue;
  margin-right: 10px ;
}

p{
  color:  $paragraph-color;
}

</style>