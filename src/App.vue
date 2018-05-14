<template>
  <v-app class="secondary">
    <v-content>
      <router-view/>
    </v-content>
    <p align="center" class="white--text ml-3">Скоро здесь будет новый крутой сайт Re:High Studio!</p>
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
