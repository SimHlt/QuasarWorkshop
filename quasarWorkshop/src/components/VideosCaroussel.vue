<template>
  <div>
    <q-carousel
      animated
      v-model="slide"
      infinite
      class="rounded-borders"
    >
      <q-carousel-slide name="soft-jazz">
        <q-video
          class="absolute-full"
          src="https://www.youtube.com/embed/k3_tw44QsZQ"
        />
      </q-carousel-slide>

      <q-carousel-slide name="Rihanna">
        <q-video
          class="absolute-full"
          src="https://www.youtube.com/embed/Dhxgf3wOIqY"
        />
      </q-carousel-slide>

      <q-carousel-slide name="ibiza">
        <q-video
          class="absolute-full"
          src="https://www.youtube.com/embed/qTsaS1Tm-Ic"
        />
      </q-carousel-slide>
    </q-carousel>

    <div class="row justify-center">
      <q-btn-toggle
        v-model="slide"
        flat
        color="white"
        toggle-color="orange"
        :options="[
          { label: 'Soft Jazz', value: 'soft-jazz' },
          { label: 'Rihanna', value: 'Rihanna' },
          { label: 'Ibiza Mix', value: 'ibiza' }
        ]"
      />
    </div>
  </div>
</template>

<script>
export default {
  name: 'VideosCaroussel',
  data () {
    return {
      slide: 'soft-jazz'
    }
  }
}
</script>

<style lang="sass">
  .q-carousel
    height: 600px
</style>
