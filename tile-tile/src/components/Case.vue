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
            <v-img height='77%' :src="require('../assets/img/case-9.jpg')"></v-img>
            <div class="case__card-title">
              <h3 color="primary">千葉県香取市個人宅</h3>
            </div>
          </v-card>
        </v-col>
        <v-col id="case-2" md='4'>
          <v-card
            hover
            height="100%"
            width="100%"
          >
            <v-img height='77%' :src="require('../assets/img/case-2.jpg')"></v-img>
            <div class="case__card-title">
              <h3 color="primary">茨城県潮来市個人宅</h3>
            </div>
          </v-card>
        </v-col>
        <v-col id="case-3" md='4'>
          <v-card
            hover
            height="100%"
          >
            <v-img height='77%' :src="require('../assets/img/case-3.jpg')"></v-img>
            <div class="case__card-title">
              <h3 color="primary">千葉県印西市美容室</h3>
            </div>
          </v-card>
        </v-col>
        <v-col id="case-4" md='4'>
          <v-card
            hover
            height="100%"
          >
            <v-img height='80%' :src="require('../assets/img/case-4.jpg')"></v-img>
            <div class="case__card-title">
              <h3 color="primary">茨城県潮来市個人宅</h3>
            </div>
          </v-card>
        </v-col>
        <v-col id="case-5" md='4'>
          <v-card
            hover
            height="100%"
          >
            <v-img height='80%' :src="require('../assets/img/case-10.jpg')"></v-img>
            <div class="case__card-title">
              <h3 color="primary">千葉県八千代市個人宅</h3>
            </div>
          </v-card>
        </v-col>
        <v-col id="case-6" md='4'>
          <v-card
            hover
            height="100%"
          >
            <v-img height='80%' :src="require('../assets/img/case-1.jpg')"></v-img>
            <div class="case__card-title">
              <h3 color="primary">千葉県某住宅展示場</h3>
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
#case-6 {
  text-align: center;
}
.case-wrapper {
  justify-content: center;
}
.case__contents {
  margin: 20px 30px 60px 30px;
  justify-content: center;
  text-align: center;
}
.case__card {
  margin: 0 70px;
  text-align: center;
  &-title {
    text-align: center;
    padding: 20px 10px 10px;
  }
  &-text {
      padding: 10px 20px;
  }
}
</style>
