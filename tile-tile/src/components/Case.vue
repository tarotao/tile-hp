<template>
  <section class="case">
    <AppBackgroundHolder :title="title" :subtitle="subtitle"/>
    <v-container fill-height class="case-wrapper">
      <v-row class="case__contents">
        <v-col id="case-1" md='4'>
          <v-card
            hover
            height="100%"
            class="case-card"
          >
            <v-img :src="require('../assets/img/ripair.png')"></v-img>
            <div class="case__card-title">
              <h3 color="primary">千葉県栄町房総のむら1</h3>
            </div>
            <div class="case__card-text">
              <p>ひび割れたタイルを補修しました。</p>
            </div>
          </v-card>
        </v-col>
        <v-col id="case-2" md='4'>
          <v-card
            hover
            height="100%"
            width="100%"
          >
            <v-img :src="require('../assets/img/ripair.png')"></v-img>
            <div class="case__card-title">
              <h3 color="primary">千葉県栄町房総のむら2</h3>
            </div>
            <div class="case__card-text">
              <p>ひび割れたタイルを補修しました。</p>
            </div>
          </v-card>
        </v-col>
        <v-col id="case-3" md='4'>
          <v-card
            hover
            height="100%"
          >
            <v-img :src="require('../assets/img/ripair.png')"></v-img>
            <div class="case__card-title">
              <h3 color="primary">千葉県栄町房総のむら3</h3>
            </div>
            <div class="case__card-text">
              <p>ひび割れたタイルを補修しました。</p>
            </div>
          </v-card>
        </v-col>
        <v-col id="case-4" md='4'>
          <v-card
            hover
            height="100%"
          >
            <v-img :src="require('../assets/img/ripair.png')"></v-img>
            <div class="case__card-title">
              <h3 color="primary">千葉県栄町房総のむら4</h3>
            </div>
            <div class="case__card-text">
              <p>ひび割れたタイルを補修しました。</p>
            </div>
          </v-card>
        </v-col>
        <v-col id="case-5" md='4'>
          <v-card
            hover
            height="100%"
          >
            <v-img :src="require('../assets/img/ripair.png')"></v-img>
            <div class="case__card-title">
              <h3 color="primary">千葉県栄町房総のむら5</h3>
            </div>
            <div class="case__card-text">
              <p>ひび割れたタイルを補修しました。</p>
            </div>
          </v-card>
        </v-col>
        <v-col id="case-6" md='4'>
          <v-card
            hover
            height="100%"
          >
            <v-img :src="require('../assets/img/ripair.png')"></v-img>
            <div class="case__card-title">
              <h3 color="primary">千葉県栄町房総のむら6</h3>
            </div>
            <div class="case__card-text">
              <p>ひび割れたタイルを補修しました。</p>
            </div>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>
<script>
import AppBackgroundHolder from './AppBackgroundHolder.vue'
import constants from '../common/constants'

export default {
  data () {
    return {
      title: 'CASE',
      subtitle: '施工実績',
      caseItems: constants.caseItems
    }
  },
  components: {
    AppBackgroundHolder
  }
}
</script>
<style lang="scss" scoped>
@import "./src/styles/common/common.scss";

.case__contents {
  margin: 20px 80px 60px 80px;
  justify-content: center;
}
.case__card {
  margin: 0 70px;
  &-title {
    text-align: center;
    padding: 20px 10px 10px;
  }
  &-text {
      padding: 10px 20px;
  }
}
</style>
