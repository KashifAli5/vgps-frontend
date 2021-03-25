<template>
  <div>
    <NavBar />
    <Slider />
    <Filters />
  <q-page-container>
  </q-page-container>
  </div>
</template>
<script>
import NavBar from '../navBar/NavBar'
import Slider from './Slider'
import Filters from './filters'

export default {
  name: 'HomeHeader',
  components: { NavBar, Slider, Filters }

}

</script>
