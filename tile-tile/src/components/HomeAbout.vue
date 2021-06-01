<template>
  <section class="home-about">
    <div class="section__title">
      <div class="section__title-text">会社概要</div>
    </div>
    <v-container>
        <v-row class="home-about__contents">
            <v-col md="5" class="home-about__contents-img">
                <img src="../assets/img/profile.jpg" alt="">
            </v-col>
            <v-col md="5" class="home-about__contents-text">
                <p>風呂場、トイレなどの水回りを始めとして、玄関周りや外壁など、経験豊富な職人による高い技術力で施工いたします。<br>「顧客満足の向上」を活動の中心に置き、お客様と信頼関係を構築し、ニーズにお応えできるよう、日々邁進しています。</p>
            </v-col>
        </v-row>
        <AppButton :button-text="buttonText" :url="url"/>
    </v-container>
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
.home-about__contents {
    margin-top: 20px;
    justify-content: center;
    &-img {
        text-align: center;
        overflow: hidden;
        height: 50vh;
    }

    &-text {
        word-wrap: break-word;
    }
}
</style>
