<template>
  <q-page class="row justify-center">
    <div  class="q-pa-xl git ">
      <TimeNavigation />
      <div class="fit row wrap justify-start items-start content-start">
          <BaseCard />
          <BaseCard /></div>
        </div>
  </q-page>
</template>

<script setup>
import TimeNavigation from 'src/components/TimeNavigation.vue'
import BaseCard from 'src/components/BaseCard.vue'
</script>
