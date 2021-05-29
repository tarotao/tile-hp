<template>
  <section class="about">
    <AppBackgroundHolder :title='title'/>
    <h2>昭和３４年設立</h2>
  </section>
</template>

<script>
import AppBackgroundHolder from './AppBackgroundHolder.vue'

export default {
  data () {
    return {
      title: 'About'
    }
  },
  components: {
    AppBackgroundHolder
  }
}
</script>
