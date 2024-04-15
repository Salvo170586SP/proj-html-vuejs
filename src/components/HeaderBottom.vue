<template>
  <div id="header-bottom">
    <div class="container">
      <div class="row align-items-center">
        <div class="col-12 col-md-5   ">
          <div class="row">
            <div class="col-12 title-section">Business Planning</div>
            <div class="col-12 subtitle-section">Digital Tecnology</div>
            <div class="col-12 title-section">Modern Solution!</div>
            <div class="col-12">
              <p class="my-2">
                When, while the lovely valley teems with vapour around meand the
                meridian sun strikes the upper surface.
              </p>
            </div>
            <div class="col-12 my-5">
              <a href="#" class="bg-red px-4">Try It Now</a>
              <a href="#" class="bg-blue px-4 ms-4">Explore More</a>
            </div>
          </div>
        </div>
        <div class="col-12 col-md-7  ">
          <img  class="img-fluid p-5" src="../assets/images/header.png" alt="header-img" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HeaderBottom",
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";

/* text */
h1 {
  margin-top: 50px;
}

span {
  font-weight: 400;
}

p {
  color: $paragraph-color;
}

.title-section {
  font-size: 3rem;
  font-weight: bold;
  color: white;
}

.subtitle-section {
  font-size: 3rem;
  color: white;
}

a {
  border-radius: 25px;
  padding: 10px 15px;
}

a.bg-red {
  background: linear-gradient(
    90deg,
    rgba(0, 29, 36, 1) 0%,
    rgba(100, 133, 145, 1) 0%,
    rgba(227, 18, 47, 1) 100%
  );
  &.bg-red:hover {
    background: linear-gradient(
      270deg,
      rgba(2, 0, 36, 1) 0%,
      rgba(36, 36, 115, 1) 0%,
      rgba(0, 160, 186, 1) 100%
    );
    color: white;
  }
}

a.bg-blue {
  background: linear-gradient(
    270deg,
    rgba(2, 0, 36, 1) 0%,
    rgba(36, 36, 115, 1) 0%,
    rgba(0, 160, 186, 1) 100%
  );
  &.bg-blue:hover {
    background: linear-gradient(
      90deg,
      rgba(0, 29, 36, 1) 0%,
      rgba(100, 133, 145, 1) 0%,
      rgba(227, 18, 47, 1) 100%
    );
    color: white;
  }
}
</style>