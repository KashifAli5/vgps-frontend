<template>
  <div class="homeSliderWrp">
    <q-carousel
      animated
      v-model="slide"
      infinite
      :autoplay="autoplay"
      arrows
      transition-prev="slide-right"
      transition-next="slide-left"
      @mouseenter="autoplay = false"
      @mouseleave="autoplay = true"
    >
      <q-carousel-slide :name="1" img-src="https://vgps.crewlogix.com/images//banners/new-banner-2.jpg"></q-carousel-slide>
      <q-carousel-slide :name="2" img-src="https://d2cv1d7fub3ij0.cloudfront.net/banner/images/2021/02/04/p_1612475587_nba-all-star-2021-NBA2021.jpg"></q-carousel-slide>
      <q-carousel-slide :name="3" img-src="https://d2cv1d7fub3ij0.cloudfront.net/banner/images/2021/02/07/p_1612720356_red-bull-1440-x-red_bull_1440.jpg"></q-carousel-slide>
      <q-carousel-slide :name="4" img-src="https://d2cv1d7fub3ij0.cloudfront.net/banner/images/2020/10/03/p_1601714157_ad3-VGPSAD3__GPS2.jpg"></q-carousel-slide>
    </q-carousel>
  </div>
</template>

<script>
export default {
  name: 'Slider',
  data () {
    return {
      slide: 1,
      autoplay: true
    }
  }

}
</script>
