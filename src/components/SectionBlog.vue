<template>
  <section id="blog">
    <div class="container">
      <div class="row text-center my-5">
        <div class="col-12">
          <span class="red-span">Blog</span>
          <h2><strong>Latest</strong> Post</h2>
          <p>
            When, while the lovely valley teems with vapour around meand the
            meridian sun strikes the upper surface.
          </p>
        </div>
      </div>
      <div class="row">
        <div class="col-6">
          <!-- card blog -->
          <div class="card-blog bg-img d-flex align-items-end p-3 text-white">
            <div class="text-card w-text">
              <span>April 21, 2019 &#8226; by Paul</span>
              <h5>Amazon gets CCI nod to aquire 49% stake in</h5>
              <p>
                When, while the lovely valley teems with vapour around meand the
                meridian sun strikes the upper surface.
              </p>
            </div>
            <div class="link-card w-link mb-5">
              <a class="bg-white" href="#">Read More</a>
            </div>
          </div>
        </div>
        <div class="col-3">
          <!-- card-blog -->
          <div class="card-blog bg-blue text-white p-5">
            <div class="text-card mb-4">
              <span>April 21, 2019 &#8226; by Paul</span>
              <h5 class="my-4">Amazon gets CCI nod to aquire 49% stake in</h5>
              <p class="my-4">
                When, while the lovely valley teems with vapour around me, the
                meridian sun s...
              </p>
            </div>
            <div class="link-card my-5">
              <a class="bg-white" href="#">Read More</a>
            </div>
          </div>
        </div>
        <div class="col-3">
          <!-- card-blog -->
          <div class="card-blog bg-blue text-white p-5">
            <div class="text-card mb-4">
              <span>April 21, 2019 &#8226; by Paul</span>
              <h5 class="my-4">Amazon gets CCI nod to aquire 49% stake in</h5>
              <p class="my-4">
                When, while the lovely valley teems with vapour around me, the
                meridian sun s...
              </p>
            </div>
            <div class="link-card my-5">
              <a class="bg-white" href="#">Read More</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "SectionBlog",
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";

#blog {
  height: 100vh;
  display: flex;
  align-items: center;
  background-color: $bg-lightwhite;

  .red-span {
    color: $red-span;
  }

  .card-blog {
    border-radius: 25px;
    height: 380px;

    &.bg-img {
      background-image: linear-gradient(rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.6)),
        url("../assets/images/headway-537308-unsplash-1380x703.jpg");
      background-position: center;
      background-size: cover;
    }

    &.bg-blue {
      background: linear-gradient(
        159deg,
        rgba(1, 3, 11, 1) 0%,
        rgba(0, 3, 25, 1) 0%,
        rgba(18, 134, 227, 1) 150%
      );
    }

    .w-text {
      width: 70%;
    }

    .w-link {
      width: 30%;
    }

    a {
      border-radius: 25px;
      padding: 10px 30px;
      &.bg-white {
        background-color: $bg-white;
        color: $txt-black;
      }
      &.bg-white:hover {
        background: linear-gradient(
          90deg,
          rgba(0, 29, 36, 1) 0%,
          rgba(100, 133, 145, 1) 0%,
          rgba(227, 18, 47, 1) 100%
        );
        color: white;
      }
    }
  }
}
</style>