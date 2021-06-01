<template>
    <section class="home">
        <HomeHero/>
        <HomeAbout/>
        <HomeWork/>
        <HomeCase/>
        <HomeRecruit/>
    </section>
</template>

<script>
import HomeHero from './HomeHero.vue'
import HomeAbout from './HomeAbout.vue'
import HomeCase from './HomeCase.vue'
import HomeWork from './HomeWork.vue'
import HomeRecruit from './HomeRecruit.vue'

export default {
  components: {
    HomeHero,
    HomeAbout,
    HomeWork,
    HomeCase,
    HomeRecruit
  }
}
</script>

<style lang="scss" scoped>
.home {
  padding-bottom: 50px;
}
</style>
