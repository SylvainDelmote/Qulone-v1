<template>
  <q-layout view="lHh lpR lFf">

    <q-header elevated class="bg-black "  >
        <q-toolbar class="row justify-evenly q-py-sm">
          <q-btn  no-caps class="q-ml-xl" icon="menu" @click="toggleLeftDrawer"> Menu</q-btn>
          <a href="/"><q-img src="../assets/logo.png"  style="height: 37px; width: 160px" fit='contain'/> </a>

          <q-btn class="q-mr-lg" icon="person" no-caps > Me connecter </q-btn>
        </q-toolbar>
        <q-page-scroller expand reverse position="top" :scroll-offset="10" :offset="[0, -10]">
          <q-toolbar inset class=" bg-black row justify-center">
            <q-tabs
              inline-label active-color="red">
              <q-tab active name="tv" icon="tv"  label="A la TV" />
              <q-separator dark vertical inset />
              <q-tab name="streaming" icon="connected_tv" label="En Streaming" />
              <q-separator dark vertical inset />
              <q-tab name="cinema" icon="movie" label="Au cinéma" />
            </q-tabs>
            <q-separator dark vertical inset />
            <q-tabs dense no-caps >
              <q-tab   name="canal" label="Canal +" />
              <q-tab  name="disney" label="Disney +" />
              <q-tab  name="salto"  label="Salto" />
              <q-tab name="prime"  label="Prime Video" />
              <q-tab name="netflix" label="Netflix" />
            </q-tabs>
          </q-toolbar>
        </q-page-scroller>
      </q-header>

    <q-drawer v-model="leftDrawerOpen" side="left" overlay behavior="desktop" elevated>
      <!-- drawer content -->
    </q-drawer>

    <q-page-container>
      <router-view />
         <q-page padding>
          <p v-for="n in 15" :key="n">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Fugit nihil praesentium molestias a adipisci, dolore vitae odit, quidem consequatur optio voluptates asperiores pariatur eos numquam rerum delectus commodi perferendis voluptate?
          </p>
          </q-page>

    </q-page-container>

    <q-footer reveal elevated class="bg-grey-8 text-white">
      <q-toolbar>

      </q-toolbar>
    </q-footer>

  </q-layout>
</template>

<script>
import { ref } from 'vue'

export default {
  setup () {
    const leftDrawerOpen = ref(false)

    return {
      leftDrawerOpen,
      toggleLeftDrawer () {
        leftDrawerOpen.value = !leftDrawerOpen.value
      }
    }
  }
}
</script>

<style>
.navbar{
display: flex;
flex-direction: row;
align-items:center;
justify-content: space-around;
background-color: blue;
}
</style>
