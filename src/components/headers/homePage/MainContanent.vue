<template>
  <div>
      <q-layout>
          <q-page-container>
              <div class="q-container customContainer">
                    <div class="row q-gutter">
                        <div class="col-md-3 q-mb-md cardCol">
                            <EventCard
                                banner='https://cdn.quasar.dev/img/mountains.jpg'
                                title='Jhay Cortez'
                                startDate='Fri, 2/26/21'
                                endDate='Fri, 2/26/21'
                                startTime='10:00 PM'
                                category='Gilt Nightclub'
                                tags='#Entertainment'
                                tagLink='#tag'
                                city='Orlando'
                                state='FL'
                                views='59'
                              />
                        </div>
                        <div class="col-md-3 q-mb-md cardCol">
                            <EventCard
                                banner='https://cdn.quasar.dev/img/mountains.jpg'
                                title='Jhay Cortez'
                                startDate='Fri, 2/26/21'
                                endDate='Fri, 2/26/21'
                                startTime='10:00 PM'
                                category='Gilt Nightclub'
                                tags='#Entertainment'
                                tagLink='#tag'
                                city='Orlando'
                                state='FL'
                                views='59'
                              />
                        </div>
                        <div class="col-md-3 q-mb-md cardCol">
                            <EventCard
                                banner='https://cdn.quasar.dev/img/mountains.jpg'
                                title='Jhay Cortez'
                                startDate='Fri, 2/26/21'
                                endDate='Fri, 2/26/21'
                                startTime='10:00 PM'
                                category='Gilt Nightclub'
                                tags='#Entertainment'
                                tagLink='#tag'
                                city='Orlando'
                                state='FL'
                                views='59'
                              />
                        </div>
                        <div class="col-md-3 q-mb-md cardCol">
                            <EventCard
                                banner='https://cdn.quasar.dev/img/mountains.jpg'
                                title='Jhay Cortez'
                                startDate='Fri, 2/26/21'
                                endDate='Fri, 2/26/21'
                                startTime='10:00 PM'
                                category='Gilt Nightclub'
                                tags='#Entertainment'
                                tagLink='#tag'
                                city='Orlando'
                                state='FL'
                                views='59'
                              />
                        </div>
                        <div class="col-md-3 q-mb-md cardCol">
                            <EventCard
                                banner='https://cdn.quasar.dev/img/mountains.jpg'
                                title='Jhay Cortez'
                                startDate='Fri, 2/26/21'
                                endDate='Fri, 2/26/21'
                                startTime='10:00 PM'
                                category='Gilt Nightclub'
                                tags='#Entertainment'
                                tagLink='#tag'
                                city='Orlando'
                                state='FL'
                                views='59'
                              />
                        </div>
                        <div class="col-md-3 q-mb-md cardCol">
                            <EventCard
                                banner='https://cdn.quasar.dev/img/mountains.jpg'
                                title='Jhay Cortez'
                                startDate='Fri, 2/26/21'
                                endDate='Fri, 2/26/21'
                                startTime='10:00 PM'
                                category='Gilt Nightclub'
                                tags='#Entertainment'
                                tagLink='#tag'
                                city='Orlando'
                                state='FL'
                                views='59'
                              />
                        </div>
                    </div>
                    <div class="homePagination q-my-lg">
                        <div class="q-pa-lg flex flex-center">
                         <q-pagination
                          v-model="current"
                          :max="5"
                          :direction-links="true"
                        >
                        </q-pagination>
                      </div>
                    </div>

              </div>
          </q-page-container>
      </q-layout>
  </div>
</template>
<script>
import EventCard from '../../layout/EventCard'
export default {
  name: 'MainContanent',
  components: { EventCard },
  data () {
    return {
      current: 1
    }
  }
}

</script>
