<template>
    <section class="home-hero">
        <v-container fluid fill-height class="home-hero__content">
        <v-row>
            <v-col class="home-hero__content-text">
                <p>50年以上の歴史が紡ぐ</p>
                <p>確かな技術力</p>
            </v-col>
        </v-row>
    </v-container>
    </section>
</template>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Sawarabi+Mincho&display=swap');
@import "./src/styles/common/common.scss";
.home-hero__content {
    background: url("../assets/img/hero-top.jpg");
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

         @include display_pc {
            font-size: 40px;
        }
    }
}
</style>
