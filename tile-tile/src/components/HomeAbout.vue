<template>
  <section class="home-about">
    <div class="section__title">
      <div class="section__title-text">01. About Me</div>
    </div>
    <v-container>
        <v-row class="home-about__contents">
            <v-col md="5" class="home-about__contents-img">
                <img src="../assets/img/profile.jpg" alt="">
            </v-col>
            <v-col md="5" class="home-about__contents-text">
                <p>##########################################</p>
                <p>@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@</p>
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
    }

    &-text {
        word-wrap: break-word;
    }
}
</style>
