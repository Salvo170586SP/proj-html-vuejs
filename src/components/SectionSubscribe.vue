<template>
  <section id="subscribe" class="d-flex align-items-center">
    <div class="container">
      <div class="row">
        <div class="col-12 d-flex">
          <div class="text-subscribe">
            Lorem ipsum dolor sit amet consectetur adipisicing elit.
            Consequuntur blanditiis velit nisi eaque sit iure nemo officiis sed,
            alias consectetur provident excepturi eos numquam repellendus
            eveniet repudiandae, veniam quas consequatur?
          </div>
          <div class="input-subscribe">
              <input type="text">
              <button>Subscribe</button>
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

.text-subscribe{
    width: 50%;
}

.input-subscribe{
    width: 50%;
    text-align: end;
}
</style>