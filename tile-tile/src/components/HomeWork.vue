<template>
    <section class="home-service">
        <div class="section__title">
            <div class="section__title-text"><span>WORK</span></div>
            <p>業務内容</p>
        </div>
        <v-container>
          <v-row class="home-service__contents">
            <v-col md="5">
              <v-card
                to="/work#work-1"
                hover
                height="100%"
              >
                <div class="home-service__card-title">
                  <h3>新築施工</h3>
                </div>
                <div class="home-service__card-img">
                  <img class="icon--service" src="../assets/img/new.png" alt="">
                </div>
                <div class="home-service__card-text">
                  <p>戸建、マンション、壁、床、あらゆるタイル工事に対応しています。</p>
                </div>
              </v-card>
            </v-col>
            <v-col md="5">
              <v-card
                to="/work#work-2"
                hover
                height="100%"
              >
                <div class="home-service__card-title">
                  <h3>補修工事</h3>
                </div>
                <div class="home-service__card-img">
                  <img class="icon--service" src="../assets/img/ripair.png" alt="">
                </div>
                <div class="home-service__card-text">
                  <p>お風呂場や、玄関、外壁などのタイルのひびや剥がれ、目地などの補修工事に対応しています。</p>
                </div>
              </v-card>
            </v-col>
          </v-row>
        </v-container>
    </section>
</template>

<style lang="scss" scoped>
@import "./src/styles/common/common.scss";

.home-service {
  margin-bottom: 100px;
}
.home-service__contents {
  margin-top: 20px;
  justify-content: center;
}

.home-service__card-title {
  text-align: center;
  padding: 20px 10px 10px;
}

.home-service__card-img {
  text-align: center;
  padding: 20px;
}

.home-service__card-text {
  padding: 10px 20px;
}

.icon--service {
  width: 48px;
  height: 48px;
}

.v-window {
  height: 300px !important;

  @include display_pc {
    height: 500px !important;
  }
}
</style>
