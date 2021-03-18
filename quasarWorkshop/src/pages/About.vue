<template>
  <q-page padding>
    <div class=" row q-pa-md">
      <div class="col-6">
        <about-component :params="paramsSimon"/>
      </div>
      <div class="col-6">
        <about-component :params="paramsMartin"/>
      </div>
    </div>
  </q-page>
</template>

<script>
import AboutComponent from 'src/components/AboutComponent.vue'
export default {
  components: { AboutComponent },
  name: 'AboutPage',
  data () {
    return {
      paramsSimon: {
        src: 'https://teameq.net/wp-content/uploads/2018/05/gandalf-3d-glasses.jpg',
        firstName: 'Simon',
        lastName: 'Houliat'
      },
      paramsMartin: {
        src: 'https://pyxis.nymag.com/v1/imgs/bde/80e/97b3659143234ec9e2fc395098f80f58d6-02-poop-emoji-debate.rsocial.w1200.jpg',
        firstName: 'Martin',
        lastName: 'Rabaud'
      }
    }
  },
  component: {
    AboutComponent: () => import('src/components/AboutComponent.vue')
  }
}
</script>

<style lang="sass">
.q-page
  background: linear-gradient(to right, #136a8a, #267871)
</style>
