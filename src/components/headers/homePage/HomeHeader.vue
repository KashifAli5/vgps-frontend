<template>
  <div>
    <NavBar />
    <Slider />
  <q-page-container>
  </q-page-container>
  </div>
</template>
<script>
import NavBar from '../navBar/NavBar'
import Slider from './Slider'

export default {
  name: 'HomeHeader',
  components: { NavBar, Slider }

}

</script>
