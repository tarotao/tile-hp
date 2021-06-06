<template>
  <section class="work">
    <AppBackgroundHolder :title="title" :subtitle="subtitle"/>
    <!-- <div class="aaa">戸建、マンション、壁、床、あらゆるタイル工事に対応しています。スピーディーな施工・納品を実現するとともに、「お施主から何を求められているか」を自分たちで考え発展させ行動にうつすこと自慢です。
           多くの建材が普及している状態ですが、タイルは今も昔も変わらずに多くの建築物に使用されています。
           外壁の張替えや、補修など幅広く対応させていただきます。是非一度ご相談下さい。
    </div> -->
    <v-container fill-height class="work-contents">
      <v-row>
        <v-col>
          <h2>新築施工</h2>
          <p>戸建、マンション、壁、床、あらゆるタイル工事に対応しています。スピーディーな施工・納品を実現するとともに、「お施主から何を求められているか」を自分たちで考え発展させ行動にうつすこと自慢です。
             多くの建材が普及している状態ですが、タイルは今も昔も変わらずに多くの建築物に使用されています。
             外壁の張替えや、補修など幅広く対応させていただきます。是非一度ご相談下さい。
          </p>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>
<script>
import AppBackgroundHolder from './AppBackgroundHolder.vue'

export default {
  data () {
    return {
      title: 'WORK',
      subtitle: '業務内容'
    }
  },
  components: {
    AppBackgroundHolder
  }
}
</script>
<style lang="scss" scoped>
// .work__contents {
//   text-align: center;
// }
.aaa {
  width: 80%;
  margin: 0 auto;
}
#work-1 {
  height: 1000px;
}

#work-2 {
  height: 1000px;
}

#work-3 {
  height: 1000px;
}
</style>
