<template>
  <section class="home-recruit">
    <div class="section__title">
      <div class="section__title-text top"><span>RECRUIT</span></div>
      <p>採用</p>
    </div>
    <v-container class="v-con">
        <v-row class="home-recruit__contents">
            <v-col md="10" class="home-recruit__contents-text">
                <p>有限会社石橋タイル工業では通年で採用を実施しています。これまでの経験を活かして活躍したい方や、新たなフィールドで知識や技術を身に着けたい方のエントリーをお待ちしています。</p>
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
      buttonText: '採用情報を詳しく見る',
      url: '/Recruit'
    }
  },
  components: {
    AppButton
  }
}
</script>

<style lang="scss" scoped>
@import "./src/styles/common/common.scss";

.home-recruit__contents {
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
.v-con {
  margin-bottom: 70px;
}
</style>
