<template>
  <v-app class="secondary">
    <v-content>
      <router-view/>
    </v-content>
    <v-footer>
      <span class="secondary--text ml-3">Скоро здесь будет клевый новый сайт!</span>
    </v-footer>
  </v-app>
</template>

<script>
  export default {
    data () {
      return {
        clipped: false,
        drawer: true,
        fixed: false,
        items: [{
          icon: 'bubble_chart',
          title: 'Inspire'
        }],
        miniVariant: false,
        right: true,
        rightDrawer: false,
        title: 'Vuetify.js'
      }
    },
    name: 'App'
  }
</script>
