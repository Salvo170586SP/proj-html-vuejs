<template>
  <div id="header-bottom">
    <div class="container">
      <div class="row align-items-center">
        <div class="col-4 pt-5">
          <div class="row">
            <div class="col-12 title-section">Business Planning</div>
            <div class="col-12 subtitle-section">Digital Tecnology</div>
            <div class="col-12 title-section">Modern Solution!</div>
            <div class="col-12">
              <p class="my-5">
                When, while the lovely valley teems with vapour around meand the
                meridian sun strikes the upper surface.
              </p>
            </div>
            <div class="col-12">
              <a href="#" class="try-btn px-4">Try It Now</a>
              <a href="#" class="explore-btn px-4 ms-4">Explore More</a>
            </div>
          </div>
        </div>

        <div class="col-8 px-5">
          <img src="../assets/images/header.png" alt="header-img" />
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

a.try-btn{
  background: rgb(0,29,36);
background: linear-gradient(90deg, rgba(0,29,36,1) 0%, rgba(100,133,145,1) 0%, rgba(227,18,47,1) 100%);
}
a.explore-btn {
 background: rgb(2,0,36);
background: linear-gradient(270deg, rgba(2,0,36,1) 0%, rgba(36,36,115,1) 0%, rgba(0,160,186,1) 100%);
}
</style>