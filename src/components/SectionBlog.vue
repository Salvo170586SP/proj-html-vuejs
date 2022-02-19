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
          <div class="card-blog d-flex align-items-end p-3 text-white">
            <div class="text-card">
              <span>April 21, 2019 by Paul</span>
              <h5>Amazon gets CCI nod to aquire 49% stake in</h5>
              <p>
                When, while the lovely valley teems with vapour around meand the
                meridian sun strikes the upper surface.
              </p>
            </div>
            <div class="link-card mb-5">
              <a class="read-btn" href="#">Read More</a>
            </div>
          </div>
        </div>
        <div class="col-3">item card</div>
        <div class="col-3">item card</div>
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
  height: 700px;
}

.red-span {
  color: $red-span;
}

.card-blog {
  height: 340px;
  background-image: url("../assets/images/headway-537308-unsplash-1380x703.jpg");
  background-position: center;
  background-size: cover;
  border-radius: 25px;
}

.text-card {
  width: 70%;
}

.link-card {
  width: 30%;
}

.read-btn {
  border-radius: 25px;
  padding: 10px 30px;
  background-color: $bg-white;
  color: $txt-black;
}
</style>