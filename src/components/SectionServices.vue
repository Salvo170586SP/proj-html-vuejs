<template>
  <section id="services" class="d-flex align-items-center">
    <div class="container">
      <!-- title -->
      <div class="row py-5">
        <div class="col-12 text-center"><span>Our Services</span></div>
        <div class="col-12 h2 text-center"><strong>What</strong> We Do</div>
        <div class="col-12 text-center">
          When wile the lovely valley teems whit vapour around meand the
        </div>
      </div>

      <!-- card services -->
      <div class="row text-center align-items-end cards-services">       
        <div class="col d-flex">
          <ServiceCards v-for="(card, index) in servicesCards" :key="index" :card="card" />
        </div>

      </div>
      <div class="row">
        <div class="col-12 text-center">
          <a class="bg-red" href="#">View All Services</a>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import ServiceCards from "../components/ServiceCards.vue";

export default {
  name: "SectionServices",
  components:{ServiceCards},
  data(){
    return{
       servicesCards:[
        {url: require('../assets/images/Group-247.png'), title: 'Data Analysis', text: 'When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper'},
        {url: require('../assets/images/Group-567.png'), title: 'Seo Optimization', text: 'When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper'},
        {url: require('../assets/images/Group-538.png'), title: 'Security Data', text: 'When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper'},
        {url: require('../assets/images/Group-566.png'), title: 'Branding strategy', text: 'When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper'},
      ],
    }
  }
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";

#services {
  height: 100vh;

  /* utility */
  span {
    color: $red-span;
  }

  /* CARD-SERVICES */
  .cards-services {
    margin-bottom: 200px;
  }

  figure {
    width: 150px;

    img {
      width: 100%;
    }
  }

  a {
    border-radius: 25px;
    padding: 10px 15px;

    &.bg-red {
      background: linear-gradient(
        90deg,
        rgba(0, 29, 36, 1) 0%,
        rgba(100, 133, 145, 1) 0%,
        rgba(227, 18, 47, 1) 100%
      );
    }
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
}
</style>