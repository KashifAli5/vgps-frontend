<template>
  <q-page-sticky expand position="top" class="z-top">
    <q-toolbar class="bg-primary text-white shadow-2 row q-py-sm q-px-lg">
    <!-- <q-btn flat round dense icon="menu" class=""></q-btn> -->
          <!-- <q-separator dark vertical inset></q-separator>
          <q-btn stretch flat label="Link"></q-btn> -->
    <!--       <div class="row">
            <div class="col-md-2 col-sm-6">
              <q-avatar>
                <img src="https://cdn.quasar.dev/logo/svg/quasar-logo.svg">
              </q-avatar>
            </div>
            <div slot="left">
              <div class="col-md-2 col-sm-6 navCitySelector">
                   <q-btn outline color="white" label="Outline"></q-btn>
              </div>
            </div>
     -->          <!-- <div class="col-md-2 col-sm-12">
                  search bar
              </div>
              <div class="col-6">
                Nav
              </div> -->
          <!-- </div> -->

            <div class="col-sm-6 col-md-1 siteLogo">
                <q-img class="siteLogoImg" src="https://d2cv1d7fub3ij0.cloudfront.net/system-images/logo.png"></q-img>
            </div>
            <div class="col-md-2 col-sm-2 navCitySelector">
                   <q-btn outline color="white" label="New York, NY"></q-btn>
              </div>
              <div class="navSearchBar col-md-4">
                <div>
                   <q-input color="white" bottom-slots v-model="text" label="search"/>
                </div>
              </div>

    </q-toolbar>
</q-page-sticky>
</template>

<script>
export default {
  name: 'NavBar'
}
</script>
