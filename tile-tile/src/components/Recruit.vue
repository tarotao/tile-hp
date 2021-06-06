<template>
  <section class="service">
    <AppBackgroundHolder :title="title" :subtitle="subtitle"/>
    <v-container fill-height>
      <v-row>
        <v-col>
          <p class="title sub">応募の際は、以下の電話番号またはメールアドレスにご連絡ください。</p>
          <ul>
            <li>電話番号:0479-82-4803</li>
            <li>メールアドレス:tarotaro0987@yahoo.co.jp</li>
          </ul>
        </v-col>
      </v-row>
      <v-row>
        <v-col>
          <h2 class="title">雇用条件</h2>
          <hr>
          <v-simple-table class="v-table">
            <template v-slot:default>
              <tbody>
                <tr
                  v-for="(recItem, index) in recItems"
                  :key="index"
                >
                  <td width="30%">{{ recItem.row }}</td>
                  <td width="70%">{{ recItem.col }}</td>
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
      title: 'RECRUIT',
      subtitle: '採用',
      recItems: constants.recruitItems
    }
  },
  components: {
    AppBackgroundHolder
  }
}
</script>
<style lang="scss" scoped>
.title {
  margin: 30px 0 10px 0;
}
.v-table {
  margin: 10px 0 80px 0;
}
</style>
