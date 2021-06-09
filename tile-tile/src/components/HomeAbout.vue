<template>
  <section class="home-about">
    <div class="section__title">
      <div class="section__title-text"><span>ABOUT</span></div>
      <p class="section__title-text-sub">会社案内</p>
    </div>
    <v-container>
      <v-row class="home-about__contents">
        <v-col cols='12' sm="5">
          <v-img class="home-about__contents-img" :src="require('../assets/img/working.jpg')"></v-img>
        </v-col>
        <v-col>
          <p class="home-about__contents-text">風呂場、トイレなどの水回りを始めとして、玄関まわりや外壁など、経験豊富な職人による高い技術力で施工いたします。</p>
          <p class="home-about__contents-text">「１２０％の満足度」を活動の中心に置き、お客様と信頼関係を構築し、ニーズにお応えできるよう、日々邁進しています。</p>
        </v-col>
      </v-row>
    </v-container>
    <AppButton :button-text="buttonText" :url="url"/>
  </section>
</template>

<script>
import AppButton from './AppButton.vue'

export default {
  data () {
    return {
      buttonText: '詳しく見る',
      url: '/about'
    }
  },
  components: {
    AppButton
  }
}
</script>

<style lang="scss" scoped>
@import "./src/styles/common/common.scss";
.home-about {
  margin-bottom: 100px;
  justify-content: center;
  &__contents {
    margin-top: 20px;
    &-img {
        text-align: center;
        max-height: 90%;
        max-width: 100%;
        margin: 0 30px 30px 30px;
    }
    &-text {
        word-wrap: break-word;
    }
  }
}
</style>
