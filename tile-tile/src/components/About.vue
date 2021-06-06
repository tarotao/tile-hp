<template>
  <section class="about">
    <AppBackgroundHolder :title='title' :subtitle="subtitle"/>
    <v-container>
      <v-row class="about__contents" >
            <v-col cols="12" sm="5">
              <v-card
                height="100%"
                class="about__card"
              >
                <div class="about__card-title">
                  <h3>新築施工</h3>
                </div>
                <div class="about__card-img">
                  <img class="icon--service" src="../assets/img/new.png" alt="">
                </div>
                <div class="about__card-text">
                  <p>戸建、マンション、壁、床、あらゆるタイル工事に対応しています。</p>
                </div>
              </v-card>
            </v-col>
            <v-col cols="12" sm="5">
              <v-card
                height="100%"
                class="about__card"
              >
                <div class="about__card-title">
                  <h3>補修工事</h3>
                </div>
                <div class="about__card-img">
                  <img class="icon--service" src="../assets/img/ripair.png" alt="">
                </div>
                <div class="about__card-text">
                  <p>お風呂場や、玄関、外壁などのタイルのひびや剥がれ、目地などの補修工事に対応しています。</p>
                </div>
              </v-card>
            </v-col>
      </v-row>
      <v-row class="about__table">
        <v-col>
          <v-row >
            <v-col>
              <h2>会社概要</h2>
              <hr>
              <v-simple-table class="v-table">
                <template v-slot:default>
                  <tbody>
                    <tr
                      v-for="(item, index) in items"
                      :key="index"
                    >
                      <td width="25%">{{ item.row }}</td>
                      <td width="75%">{{ item.col }}</td>
                    </tr>
                  </tbody>
                </template>
              </v-simple-table>
            </v-col>
          </v-row>
          <v-row class="about__table-his">
            <v-col>
              <h2>沿革</h2>
              <hr>
              <v-simple-table class="v-table">
                <template v-slot:default>
                  <tbody>
                    <tr
                      v-for="(hisItem, index) in hisItems"
                      :key="index"
                    >
                      <td width="30%">{{ hisItem.row }}</td>
                      <td width="70%">{{ hisItem.col }}</td>
                    </tr>
                  </tbody>
                </template>
              </v-simple-table>
            </v-col>
          </v-row>
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
      title: 'ABOUT',
      subtitle: '会社案内',
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
@import "./src/styles/common/common.scss";

.about {
  margin-bottom: 100px;
  &__contents {
    margin-top: 20px;
    justify-content: center;
  }
  &__card {
    margin: 0 45px;
    &-title {
      text-align: center;
      padding: 20px 10px 10px;
    }
    &-img {
      text-align: center;
      padding: 20px;
    }
    &-text {
      padding: 10px 20px;
      word-wrap: break-word;
    }
  }
  &__table {
    margin: 100px 0 70px 0;
    &-his {
      margin-top: 100px;
    }
  }
}

.icon--service {
  width: 48px;
  height: 48px;
}

.v-window {
  height: 300px !important;

  @include display_pc {
    height: 500px !important;
  }
}
.about__table {
  margin: 100px 0 20px 0;
  &-his {
    margin-top: 100px;
  }
}
</style>
