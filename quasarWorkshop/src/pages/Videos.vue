<template>
  <q-page>
    <div class="q-pa-xl row justify-center">
      <q-responsive :ratio="16/9" style="width: 1000px; max-width: 100%;">
        <videos-caroussel></videos-caroussel>
      </q-responsive>
    </div>
  </q-page>
</template>

<script>
import VideosCaroussel from 'components/VideosCaroussel.vue'
export default {
  components: { VideosCaroussel },
  name: 'VideosPage',
  component: {
    VideosCaroussel: () => import('components/VideosCaroussel.vue')
  }
}
</script>

<style lang="sass">
.q-page
  background: linear-gradient(to right, #136a8a, #267871)
</style>
