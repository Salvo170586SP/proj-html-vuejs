<template>
  <section id="price-list">
    <div class="container">
      <div class="row text-center py-5">
        <div class="col-12"><span class="red-span">Price List</span></div>
        <div class="col-12 h2 text-white">Our Pricing</div>
        <div class="col-12 text-white">
          When, while the lovely valley teems with vapour around meand the
          meridian sun strikes the upper surface.
        </div>
      </div>

      <div class="row text-center">
        <!-- card-price -->
        <div class="col-4 bg-white radius-25">
          <div class="row">
            <div class="col-12 py-3">
              <h2>Designing</h2>
              <p>PROCESS</p>
            </div>
          </div>
          <div class="row">
            <div class="col-12">
              <span class="size-price"> 40</span>
              <p>per Month</p>
            </div>
            <div class="col-12">
              <ul>
                <li><strong>Creative</strong> Design Enable</li>
                <li><strong>Vibrant</strong> Color Usage</li>
                <li><strong>Eye</strong> Catching Design</li>
                <li><strong>Extreme</strong> Typography</li>
                <li><strong>Exceptional</strong> Design</li>
              </ul>
            </div>
            <div class="col-12 my-5">
              <a class="order-btn" href="#">Order Now</a>
            </div>
          </div>
        </div>
        
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "SectionPrice",
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";
#price-list {
  height: 850px;
  background-image: linear-gradient(to bottom, $bg-blue 60%, white 50%);
}

.red-span {
  color: $red-span;
}

.size-price {
  font-size: 9rem;
  font-weight: bold;
}

ul {
  line-height: 35px;
}

.radius-25 {
  border-radius: 25px;
}

a {
  border-radius: 25px;
  padding: 10px 15px;
}

.order-btn {
  background-color: $red-span;
}
</style>