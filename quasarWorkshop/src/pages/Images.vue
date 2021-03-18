<template>
  <q-page class="q-pa-md">
    <div class="q-pa-xl row justify-center">
      <q-responsive :ratio="16/9" style="width: 800px; max-width: 100%;">
        <images-caroussel></images-caroussel>
      </q-responsive>
    </div>
  </q-page>
</template>

<script>

import ImagesCaroussel from 'src/components/ImagesCaroussel.vue'

export default {
  components: { ImagesCaroussel },
  name: 'ImagesPage',
  component: {
    ImagesCaroussel: () => import('components/ImagesCaroussel.vue')
  }
}
</script>

<style lang="sass">
.q-page
  background: linear-gradient(to right, #136a8a, #267871)
</style>
