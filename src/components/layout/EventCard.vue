<template>
  <div class="eventCardItem">
    <q-card class="my-card q-ma-md">
      <q-img src="https://cdn.quasar.dev/img/mountains.jpg">
        <div class="absolute-bottom">
           <span class="cardTag"> {{tags}} </span>
           <span class="cardViews q-mx-xs"> <q-icon class="q-px-xs" name="fa fa-eye"></q-icon> {{views}} </span>
           <span class="cardlikeIt q-mr-sm"> <q-icon class="q-px-xs" name="fa fa-heart"></q-icon> </span>
        </div>
      </q-img>
    <q-card-section>
      <div class="cardHeading"> {{title}} </div>
      <div class="cardDates q-mt-xs cardText">
        <span> {{startDate}} </span> - <span> {{endDate}} </span>
      </div>
      <div class="startTime q-mt-xs cardText">
        <span> Start Time: {{startTime}} </span>
      </div>
      <div class="cardTagLink q-mt-xs">
        <q-side-link tag="a" to="/some/route"> <q-item-main>{{category}}</q-item-main>  </q-side-link>
      </div>
      <div class="cardAddress cardText">
        <span> {{city}} </span>, <span> {{state}} </span>
      </div>
      <div class="cardHashtags">
        <span> {{tags}} </span>
      </div>
    </q-card-section>
  </q-card>
     <div class="cardBtnsWrp q-ml-md">
     <div class="cardFollowBtn q-mr-md">
        <q-btn label="Follow" icon="star"></q-btn>
     </div>
     <div class="cardFollowBtn">
        <q-btn label="Share" icon="share"></q-btn>
     </div>
   </div>
  </div>
</template>
<script>
export default {
  name: 'EventCard',
  props: ['title', 'startDate', 'endDate', 'startTime', 'category', 'tags', 'tagLink', 'city', 'state', 'views']
}
</script>
