<template>
  <section class="home-case">
    <div class="section__title">
      <div class="section__title-text"><span>CASE</span></div>
      <p class="section__title-text-sub">施工実績</p>
    </div>
    <v-container>
      <v-row class="home-case__contents">
        <v-col sm="8" class="home-case__contents-img">
          <v-carousel
            hide-delimiters
            height="auto"
          >
            <v-carousel-item
              v-for="(caseItem, index) in caseItems"
              :key="index"
              :to="caseItem.url"
            >
              <img :src="caseItem.src" alt="" class="img-fluid">
            </v-carousel-item>
          </v-carousel>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>

<script>
import constants from '../common/constants'

export default {
  data () {
    return {
      caseItems: constants.caseItems
    }
  }
}
</script>
<style  lang="scss" scoped>
.home-case {
  margin-bottom: 100px;
  &__contents {
    margin: 30px;
    justify-content: center;
    &-img {
      text-align: center;
    }
  }
}
</style>

<style lang="scss" scoped>
@import "./src/styles/common/common.scss";
</style>
