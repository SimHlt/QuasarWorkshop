<template>
  <q-layout view="lHh lpr lFf">
    <q-header>
      <q-toolbar>
        <q-avatar class="q-pa-md">
          <img src="https://cdn.quasar.dev/logo/svg/quasar-logo.svg">
        </q-avatar>
      </q-toolbar>
      <q-tabs>
        <q-route-tab name="images" label="Images" icon="photo" to="/images"/>
        <q-route-tab name="videos" label="Videos" icon="movie" to="/videos"/>
        <q-route-tab name="about" label="About" icon="menu_book" to="/about"/>
      </q-tabs>
    </q-header>
    <q-page-container>
      <!-- This is where pages get injected -->
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
export default {
  name: 'MainLayout',
  data () {
    return {}
  }
}
</script>

<style lang="sass">
  .q-header
    background: linear-gradient(to right, #136a8a, #267871)
</style>
