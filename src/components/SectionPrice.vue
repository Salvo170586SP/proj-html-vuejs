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
        <div class="col-4">
          <div class="card-price bg-white radius-25 p-2">
            <span class="bg-numb">40</span>
            <div class="row">
              <div class="col-12 py-3 z-index">
                <h2>Designing</h2>
                <p>PROCESS</p>
              </div>
            </div>
            <div class="row">
              <div class="col-12 z-index">
                <span class="size-price"> 40</span>
                <p>Per Month</p>
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
                <a class="red-btn fw-bold" href="#"
                  >Order Now <i class="fa-solid fa-right-long ms-4"></i
                ></a>
              </div>
            </div>
          </div>
        </div>

        <div class="col-4">
          <div class="card-price red-card text-white radius-25 p-2">
            <span class="bg-numb">60</span>
            <div class="row">
              <div class="col-12 py-3 z-index">
                <h2>Developing</h2>
                <p>PRODUCT</p>
              </div>
            </div>
            <div class="row">
              <div class="col-12 z-index">
                <span class="size-price">60</span>
                <p>Per Month</p>
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
                <a class="order-btn-white fw-bold" href="#"
                  >Order Now <i class="fa-solid fa-right-long ms-4"></i
                ></a>
              </div>
            </div>
          </div>
        </div>

        <div class="col-4">
          <div class="card-price bg-white radius-25 p-2">
            <span class="bg-numb">80</span>
            <div class="row">
              <div class="col-12 py-3 z-index">
                <h2>Supporting</h2>
                <p>CLIENTS</p>
              </div>
            </div>
            <div class="row">
              <div class="col-12 z-index">
                <span class="size-price"> 80</span>
                <p>Per Month</p>
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
                <a class="red-btn fw-bold" href="#"
                  >Order Now <i class="fa-solid fa-right-long ms-4"></i
                ></a>
              </div>
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

  .card-price {
    position: relative;

    .bg-numb {
      font-size: 18rem;
      font-weight: bold;
      color: darkgray;
      opacity: 0.3;
      position: absolute;
      top: -128px;
      right: -7px;
    }

    .z-index{
      z-index: 1;
    }
  }

  .red-card {
    background: rgb(0, 29, 36);
    background: linear-gradient(
      153deg,
      rgba(0, 29, 36, 1) 0%,
      rgba(100, 133, 145, 1) 0%,
      rgba(227, 18, 47, 1) 100%
    );
  }

  .red-span {
    color: $red-span;
  }

  .size-price {
    font-size: 6rem;
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
    padding: 10px 25px;
    &.red-btn {
      background: rgb(0, 29, 36);
      background: linear-gradient(
        90deg,
        rgba(0, 29, 36, 1) 0%,
        rgba(100, 133, 145, 1) 0%,
        rgba(227, 18, 47, 1) 100%
      );
    }
    &.order-btn-white {
      background-color: white;
      color: $red-span;
    }
  }
}
</style>