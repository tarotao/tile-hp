<template>
    <section class="home-hero">
        <v-container fluid fill-height class="home-hero__content">
        <v-row>
            <v-col class="home-hero__content-text">
                <p>半世紀以上の歴史からくる</p>
                <p>安心と信頼の施工をいたします</p>
            </v-col>
        </v-row>
    </v-container>
    </section>
</template>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Sawarabi+Mincho&display=swap');
@import "./src/styles/common/common.scss";
.home-hero__content {
    background: url("../assets/img/home-hero2.jpg");
    background-size: cover;
    background-position: center center;
    width: 100%;
    height: 50vh;

    @include display_pc {
        height: 100vh;
    }

    &-text {
        color: white;
        text-align: center;
        font-size: 28px;
        font-weight: bold;
        font-family: 'Sawarabi Mincho', sans-serif;
    }
}
</style>
