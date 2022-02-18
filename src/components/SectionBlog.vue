<template>
  <section id="blog">
    <div class="container">
      <div class="row text-center my-5">
        <div class="col-12">
          <span>Blog</span>
          <h2><strong>Latest</strong> Post</h2>
          <p>
            When, while the lovely valley teems with vapour around meand the
            meridian sun strikes the upper surface.
          </p>
        </div>
      </div>
      <div class="row">
        <div class="col-6">item card</div>
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

#blog{
    height: 700px;
}
</style>