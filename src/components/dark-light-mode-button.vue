<template>
  <div>
    <q-page-sticky position="bottom-right" :offset="[40, 40]">
       <q-btn flat round
          @click="$q.dark.toggle()"
          :icon="$q.dark.isActive ? 'nights_stay' : 'wb_sunny'"
          :class="$q.dark.isActive ? 'darkTextColor' : 'bg-primary'"
        />
    </q-page-sticky>
  </div>
</template>
<script>
export default {
  name: 'darkLightMode'
}
</script>
