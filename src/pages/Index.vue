<template>
  <q-page class="">
    <HomeHeader />
    <MainContent />
    <CityFilter />
    <Footer />
  </q-page>

</template>

<script>
import HomeHeader from '../components/headers/homePage/HomeHeader'
import MainContent from '../components/headers/homePage/MainContanent'
import CityFilter from '../components/home/CityFilter'
import Footer from '../components/footer/Footer'

export default {
  name: 'PageIndex',
  components: { HomeHeader, MainContent, Footer, CityFilter }
}
</script>
