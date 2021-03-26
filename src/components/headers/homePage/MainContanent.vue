<template>
  <div>
      <q-layout>
          <q-page-container>
              <div class="q-container customContainer">
                    <div class="row q-gutter">
                        <div class="col-md-3 q-mb-md cardCol" v-for="card in cardData"  :key="card.title">
                            <EventCard
                                banner='https://cdn.quasar.dev/img/mountains.jpg'
                                :title="card.title"
                                :startDate='card.startDate'
                                :endDate='card.endDate'
                                :startTime='card.startTime'
                                :category='card.category'
                                :tags='card.tags'
                                :tagLink='card.tagLink'
                                :city='card.city'
                                :state='card.state'
                                viewsviews='card.views'
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
                  <darkLightMode />
              </div>
          </q-page-container>
      </q-layout>
  </div>
</template>
<script>
import EventCard from '../../layout/EventCard'
import darkLightMode from '../../dark-light-mode-button'
export default {
  name: 'MainContanent',
  components: { EventCard, darkLightMode },
  data () {
    return {
      cardData: [
        { title: 'Jhay Cortez', startDate: 'Fri, 2/26/21', endDate: 'Fri, 2/26/21', startTime: '10:00 PM', category: 'Gilt Nightclub', tags: '#Entertainment', tagLink: '#tag', city: 'Orlando', state: 'FL', views: '59' },
        { title: 'JDisciple', startDate: 'Fri, 2/26/21', endDate: 'Fri, 2/26/21', startTime: '10:00 PM', category: 'Nos Event Center', tags: '#Entertainment', tagLink: '#Festival', city: 'San Bernardino', state: 'CA', views: '59' },
        { title: 'JDisciple', startDate: 'Fri, 2/26/21', endDate: 'Fri, 2/26/21', startTime: '10:00 PM', category: 'Nos Event Center', tags: '#Entertainment', tagLink: '#Festival', city: 'San Bernardino', state: 'CA', views: '59' },
        { title: 'JDisciple', startDate: 'Fri, 2/26/21', endDate: 'Fri, 2/26/21', startTime: '10:00 PM', category: 'Nos Event Center', tags: '#Entertainment', tagLink: '#Festival', city: 'San Bernardino', state: 'CA', views: '59' },
        { title: 'JDisciple', startDate: 'Fri, 2/26/21', endDate: 'Fri, 2/26/21', startTime: '10:00 PM', category: 'Nos Event Center', tags: '#Entertainment', tagLink: '#Festival', city: 'San Bernardino', state: 'CA', views: '59' },
        { title: 'JDisciple', startDate: 'Fri, 2/26/21', endDate: 'Fri, 2/26/21', startTime: '10:00 PM', category: 'Nos Event Center', tags: '#Entertainment', tagLink: '#Festival', city: 'San Bernardino', state: 'CA', views: '59' }
      ],
      current: 1
    }
  }
}

</script>
