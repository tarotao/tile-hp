<template>
  <section class="service">
    <AppBackgroundHolder :title="title"/>
    <div id="case-1">
      <h2>住宅</h2>
      <p>XXXXXXXXXXXXXXXXXXXXXXXXXXXX</p>
    </div>
    <div id="case-2">
      <h2>店舗・施設</h2>
      <p>XXXXXXXXXXXXXXXXXXXXXXXXXXXX</p>
    </div>
    <div id="case-3">
      <h2>補修</h2>
      <p>XXXXXXXXXXXXXXXXXXXXXXXXXXXX</p>
    </div>
  </section>
</template>
<script>
import AppBackgroundHolder from './AppBackgroundHolder.vue'

export default {
  data () {
    return {
      title: '実績紹介'
    }
  },
  components: {
    AppBackgroundHolder
  }
}
</script>
<style lang="scss" scoped>
#direction {
  height: 1000px;
}

#coding {
  height: 1000px;
}

#design {
  height: 1000px;
}
</style>
