<template>
  <q-page-sticky expand position="top" class="z-top">
    <q-toolbar class="bg-primary text-white shadow-2 row q-py-sm q-px-lg">

        <div class=" siteLogo">
            <q-img class="siteLogoImg" src="https://d2cv1d7fub3ij0.cloudfront.net/system-images/logo.png"></q-img>
        </div>
        <div class="navCitySelector">
               <q-btn outline color="white" label="New York, NY"></q-btn>
          </div>
          <div class="navSearchBar row justify-between">
            <div class="navSearchBlock">
               <q-input color="white" bottom-slots v-model="text" label="search"/>
            </div>
          </div>
          <div class="">
            <q-btn flat round
              @click="$q.dark.toggle()"
              :icon="$q.dark.isActive ? 'nights_stay' : 'wb_sunny'"
              :class="$q.dark.isActive ? 'darkTextColor' : 'bg-primary'"
            />
          </div>
          <div class="menuLinks justify-between ">
            <div class="navLinksBlock">
              <q-item clickable  class="active">
                 <a href="#">Home</a>
              </q-item>
              <q-item clickable >
                <a href="#" >Directory</a>
              </q-item>
              <q-item clickable >
                 <a href="#">Map</a>
              </q-item>
               <q-item clickable >
                 <a href="#">Signin</a>
              </q-item>
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
