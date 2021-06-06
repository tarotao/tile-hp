<template>
    <section>
       <AppBackgroundHolder :title="title" :subtitle="subtitle"/>
       <iframe class="v-form" src="https://docs.google.com/forms/d/e/1FAIpQLSeuKYw0QtPEtz9YF89VR_cuVrVpX_kp_TW6wqHBKwKZOGzEWA/viewform?embedded=true" width="100%" height="1000px" frameborder="0" marginheight="0" marginwidth="0" scrolling="no">読み込んでいます…</iframe>
        <!-- <iframe src="https://docs.google.com/forms/d/e/1FAIpQLSeuKYw0QtPEtz9YF89VR_cuVrVpX_kp_TW6wqHBKwKZOGzEWA/viewform?embedded=true" width="640" height="1015" frameborder="0" marginheight="0" marginwidth="0">読み込んでいます…</iframe> -->
    </section>
</template>

<script>
import AppBackgroundHolder from './AppBackgroundHolder.vue'

export default {
  data () {
    return {
      title: 'CONTACT',
      subtitle: 'お問い合わせ'
    }
  },
  components: {
    AppBackgroundHolder
  }
}
</script>
<style lang="scss" scoped>
.v-form {
    padding-bottom: 60px;
}
</style>
