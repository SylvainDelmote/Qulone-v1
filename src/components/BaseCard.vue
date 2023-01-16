<template>
<q-card  class="   my-card" flat bordered>
  <q-card-section row horizontal justify-between>
    <q-card-section class="q-pt-xs">
      <div class="text-overline text-weight-bold q-mt-sm q-mb-xs">21h10</div>
      <div class="text-subtitle2 text-weight-bold q-mt-sm q-mb-xs">Les Tuche 3</div>
      <div class="text-caption text-grey">Cinema</div>
      <div class="text-caption text-grey">1h45min</div>
    </q-card-section>
    <q-card-section class="col-4 flex items-stretch">
      <q-img class="rounded-borders" src="https://cdn.quasar.dev/img/parallax2.jpg"/>
    </q-card-section>
  </q-card-section>
  </q-card>
</template>

<script setup>

</script>

<style lang="scss" scoped>
.my-card{
  overflow: auto; min-height: 120px; max-height: 120px;  min-width: 265px; max-width: 265px;
}

</style>
