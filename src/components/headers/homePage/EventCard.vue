<template>
    <div class="eventCardItem">
    	<q-card class="my-card q-ma-md">
        <q-img src="https://cdn.quasar.dev/img/mountains.jpg">
            <div class="absolute-bottom">
                <span> Night life </span>
            </div>
        </q-img>

        <q-card-section>
            <div class="text-h6">Our Changing Planet</div>
            <div class="text-subtitle2">by John Doe</div>
        </q-card-section>

        <q-card-section class="q-pt-none">
            {{ lorem }}
        </q-card-section>
    </q-card>
    </div>
</template>
<script>
export default {
  name: 'EventCard'
}
</script>
