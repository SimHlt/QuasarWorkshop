<template>
    <q-carousel
      animated
      v-model="slide"
      arrows
      navigation
      infinite
      class="rounded-borders"
    >
      <q-carousel-slide :name="1" img-src="https://cdn.quasar.dev/img/mountains.jpg" />
      <q-carousel-slide :ratio="16/9" :name="2" img-src="https://yt3.ggpht.com/trPPy7gdAJP7koF2uzJmZv3QygCy72qTYS_D008KVROtsCCifHrgj1r3T_W33aNADjnlbwyxsXzw=s953-nd" />
      <q-carousel-slide :name="3" img-src="https://cdn.quasar.dev/img/parallax2.jpg" />
      <q-carousel-slide :name="4" img-src="https://cdn.quasar.dev/img/quasar.jpg" />
    </q-carousel>
</template>

<script>
export default {
  name: 'ImagesCaroussel',
  data () {
    return {
      slide: 1
    }
  }
}
</script>

<style lang="sass">
.q-carousel-slide
  background-size: contain
</style>
