<template>
  <section id="blog">
    <div class="container">
      <!-- title -->
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
        <div class="col-12 col-md-6 my-2">
          <!-- card blog -->
          <div class="card-blog bg-img d-flex flex-column flex-md-row align-items-start align-items-md-end justify-content-center p-5 text-white">
            <div class="text-card w-text d-flex flex-column">
              <span>April 21, 2019 &#8226; by Paul</span>
              <h5>Amazon gets CCI nod to aquire 49% stake in</h5>
              <p>
                When, while the lovely valley teems with vapour around meand the
                meridian sun strikes the upper surface.
              </p>
            </div>
            <div class="w-100 link-card w-link my-5 mx-md-5">
              <a class="w-100 bg-white" href="#">Read More</a>
            </div>
          </div>
        </div>
        <!--  card blue -->
        <BlueCard v-for="(card, index) in blueCards" :key="index" :card="card" />
      </div>
    </div>
  </section>
</template>

<script>
import BlueCard from "../components/BlueCard.vue";

export default {
  name: "SectionBlog",
  components:{ BlueCard },
  data(){
    return{
      blueCards:[
        {date:"April 21, . by Paul", title:"Amazon gets CCI nod to aquire 49% stake in", text:"When, while the lovely valley teems with vapour around me, the meridian sun s..."},
        {date:"April 21, 2019 . by Paul", title:"Amazon gets CCI nod to aquire 49% stake in", text:"When, while the lovely valley teems with vapour around me, the meridian sun s..."},
        ],
    }
  }
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";

#blog {
  /* height: 100vh; */
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