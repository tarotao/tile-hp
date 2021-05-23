<template>
  <v-app>
    <header>
      <v-app-bar
          app
          dark
      >
        <v-app-bar-nav-icon @click="drawer = true"></v-app-bar-nav-icon>
        <v-toolbar-title>石橋タイル工業</v-toolbar-title>
        <v-tabs>
          <v-tab
            v-for="(menuItem, index) in menuItems"
            :key="index"
          >
            {{ menuItem.name }}
          </v-tab>
        </v-tabs>
      </v-app-bar>
      <v-navigation-drawer
        v-model="drawer"
        fixed
        temporary
      >
        <v-list
          nav
          dense
        >
          <v-list-group>
            <v-list-item
              v-for="(menuItem, index) in menuItems"
              :key="index"
            >
              <v-list-item-title>{{ menuItem.name }}</v-list-item-title>
            </v-list-item>
          </v-list-group>
        </v-list>
      </v-navigation-drawer>
    </header>
  </v-app>
</template>

<script>
import constants from './common/constants'
export default {
  data () {
    return {
      drawer: false,
      menuItems: constants.menuItems
    }
  }
}
</script>

<style scoped>

</style>
