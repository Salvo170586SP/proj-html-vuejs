<template>
  <section id="subscribe" class="d-flex align-items-center">
    <div class="container">
      <div class="row">
        <div class="col-12">
          <!-- card-subscribe -->
          <div class="card-subscribe text-white d-flex align-items-center">
            <div class="text-subscribe px-5">
              <h2>We Offer Awesome Services</h2>
              <p>
                When, while the lovely valley teems with vapour around meand the
                meridian sun strikes the upper surface.
              </p>
            </div>
            <div class="input-subscribe">
              <input type="text" placeholder="Enter Your Mail Address" />
              <button class="bg-blue">Subscribe</button>
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
  background-image: linear-gradient(to bottom, $bg-white 50%, $bg-blue 50%);
}

.card-subscribe {
  height: 260px;
  background: rgb(0,29,36);
background: linear-gradient(90deg, rgba(0,29,36,1) 0%, rgba(100,133,145,1) 0%, rgba(227,18,47,1) 100%);
  border-radius: 30px;
}

.text-subscribe {
  width: 70%;
}

h2 {
  font-size: 3rem;
  font-weight: 700;
}

.input-subscribe {
  width: 365px;
  text-align: end;
  background-color: $bg-white;
  border-radius: 25px;
  padding: 5px;
}

input {
  width: 250px;
  outline: none;
  border: 0;
}

button {
  border-radius: 25px;
  padding: 8px;
  border: none;
}

button.bg-blue {
background: rgb(2,0,36);
background: linear-gradient(270deg, rgba(2,0,36,1) 0%, rgba(36,36,115,1) 0%, rgba(0,160,186,1) 100%);
  color: $bg-white;
}
</style>