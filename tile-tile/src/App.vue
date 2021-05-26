<template>
  <v-app>
    <AppHeader/>
    <v-content>
      <router-view/>
    </v-content>
    <AppFooter/>
  </v-app>
</template>

<script>
import AppHeader from './components/AppHeader.vue'
import AppFooter from './components/AppFooter.vue'

export default {
  name: 'App',
  components: {
    AppHeader,
    AppFooter
  }
}
</script>
