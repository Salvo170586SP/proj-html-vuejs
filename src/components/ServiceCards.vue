<template>
  <div class="row">
            <div class="col-12 d-flex justify-content-center">
              <figure>
                <img :src="card.url" alt="data analysis" />
              </figure>
            </div>
            <div class="col-12 h3">{{card.title}}</div>
            <div class="col-12">
              <p>
               {{card.text}}
              </p>
            </div>
          </div>
</template>

<script>
export default {
name: 'ServiceCard',
props:['card']
}
</script>

<style>

</style>