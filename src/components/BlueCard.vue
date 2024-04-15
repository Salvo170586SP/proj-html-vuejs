<template>
  <!-- card-blog blue -->
         <div class="col-12 col-md-3 my-2">
          <div class="card-blog bg-blue text-white p-5">
            <div class="text-card mb-4">
              <span>{{card.date}}</span>
              <h5 class="my-4">{{card.title}}</h5>
              <p class="my-4">
                {{card.text}}
              </p>
            </div>
            <div class="link-card my-5">
              <a class="bg-white" href="#">Read More</a>
            </div>
          </div>
        </div>
</template>

<script>
export default {
name: 'BlueCard',
props: ['card'],
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";

.card-blog {
    border-radius: 25px;
    height: 380px;

    &.bg-blue {
      background: linear-gradient(
        159deg,
        rgba(1, 3, 11, 1) 0%,
        rgba(0, 3, 25, 1) 0%,
        rgba(18, 134, 227, 1) 150%
      );
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
</style>