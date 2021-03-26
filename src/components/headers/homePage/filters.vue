<template>
  <div class="">
       <q-tabs
        v-model="tab"
        inline-label
        class="bg-primary text-white shadow-2"
      >
        <q-tab name="Trending" label="Trending"></q-tab>
        <q-tab name="All" label="All"></q-tab>
        <q-tab name="Thisweek" label="This week"></q-tab>
        <q-tab name="NightLife" label="Night Life"></q-tab>
        <q-tab name="Entertainment" label="Entertainment"></q-tab>
        <q-tab name="National" label="National"></q-tab>
         <q-tab name="Festivals" label="Festivals"></q-tab>
          <q-tab name="MC/SC/CC" label="MC/SC/CC"></q-tab>
           <q-tab name="Sports" label="Sports"></q-tab>
            <q-tab name="Media" label="Media"></q-tab>

      </q-tabs>
      <div class="customContainer q-pt-lg">
      <div class="dateSelector" style="max-width: 300px">
        <q-input filled v-model="date" mask="date" :rules="['date']">
        <template v-slot:append>
          <q-icon name="event" class="cursor-pointer">
            <q-popup-proxy ref="qDateProxy" transition-show="scale" transition-hide="scale">
              <q-date v-model="date" range today-btn>
                <div class="row items-center justify-end">
                  <q-btn v-close-popup label="Close" color="primary" flat></q-btn>
                </div>
              </q-date>
            </q-popup-proxy>
          </q-icon>
        </template>
      </q-input>
      </div>
      </div><!-- end of container -->
  </div>
</template>

<script>
export default {
  name: 'Filters',
  data () {
    return {
      tab: 'Trending'
    }
  }
}
</script>
