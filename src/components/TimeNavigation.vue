<template>
  <div class="row justify-center">
  <q-banner class="bg-grey-2 ">
    <div class="text-h5 text-weight-bold q-mt-sm q-mb-xs">Programme TV</div>
    <p>Changer de date et d'heure <span class="chevron">>></span></p>
    <div class="q-gutter-y-md" style="max-width: 600px">
      <q-tabs
        v-model="tab"
        dense
        class="bg-white text-dark"
      >
        <q-tab name="hier"  label="Hier" />
        <q-tab name="now"  label="En ce moment" />
        <q-tab name="tonight" label="Ce soir " />
        <q-tab name="demain" label="Demain" />
      </q-tabs>

      </div>

  </q-banner>
  </div>
</template>

<script setup>

</script>

<style>
.chevron{
  color: red;
}
</style>
