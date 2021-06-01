<template>
  <section class="about">
    <AppBackgroundHolder :title='title'/>
    <v-container fill-height>
      <v-row>
        <v-col xl="12" lg="12" md="12" sm="12" xs="12">
          <h2 class="title">基本情報</h2>
          <hr>
          <v-simple-table class="v-table">
            <template v-slot:default>
              <tbody>
                <tr
                  v-for="item in items"
                  :key="item"
                >
                  <td>{{ item.row }}</td>
                  <td>{{ item.col }}</td>
                </tr>
              </tbody>
            </template>
          </v-simple-table>
        </v-col>
      </v-row>
      <v-row>
        <v-col>
          <h2 class="title">沿革</h2>
          <hr>
          <v-simple-table class="v-table">
            <template v-slot:default>
              <tbody>
                <tr
                  v-for="hisItem in hisItems"
                  :key="hisItem"
                >
                  <td>{{ hisItem.row }}</td>
                  <td>{{ hisItem.col }}</td>
                </tr>
              </tbody>
            </template>
          </v-simple-table>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>

<script>
import AppBackgroundHolder from './AppBackgroundHolder.vue'
import constants from '../common/constants.js'
export default {
  data () {
    return {
      title: '会社概要',
      items: constants.aboutItems,
      hisItems: constants.historyItems
    }
  },
  components: {
    AppBackgroundHolder
  }
}
</script>

<style lang="scss" scoped>
// .about {
//   width: 100%;
//   margin: 0 auto;
// }
.v-table {
  // text-align: center;
  margin: 10px 0 70px 0;
}
</style>
