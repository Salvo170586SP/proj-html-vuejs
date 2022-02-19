<template>
  <section id="subscribe" class="d-flex align-items-center">
    <div class="container">
      <div class="row">
        <div class="col-12">

            <!-- card-subscribe -->
          <div class="card-subscribe text-white d-flex align-items-center">
            <div class="text-subscribe">
              <h2>We Offer Awesome Services</h2>
              <p>
                When, while the lovely valley teems with vapour around meand the
                meridian sun strikes the upper surface.
              </p>
            </div>
            <div class="input-subscribe">
              <input type="text" />
              <button>Subscribe</button>
            </div>
          </div>

        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "SectionSubscribe",
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";

#subscribe {
  height: 400px;
  background-image: linear-gradient(to bottom, white 50%, $bg-blue 50%);
}

.card-subscribe{
    height: 300px;
    background-color: $red-span;
    border-radius: 30px;
}

.text-subscribe {
  width: 50%;
}

.input-subscribe {
  width: 50%;
  text-align: end;
}
</style>