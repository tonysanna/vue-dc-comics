<template>
    <main>
        <div class="main-top">
            <div class="icon-main">
                <div class="icon" v-for="(card,index) in cards" :key="index">
                    <div class="img-cont">
                        <img :src="card.thumb" alt="card.series">
                    </div>
                    <span>{{card.series}}</span>
                </div>
            </div>
        </div>
        <div class="main-bott">
            <ul>
                <li v-for="(icon,index) in icons" :key="index">
                    <img :src="require(`../assets/img/${icon.url + icon.path + icon.extension}`)" :alt="icon.text">
                    <span>{{icon.text}}</span>
                </li>
            </ul>
        </div>
    </main>
</template>

<script>
import cards from '@/data/dc-comics.js'

export default {
    name:'Main',

    data() {
         return {
          icons: [
                {
                    url: 'buy-comics',
                    path: '-digital-comics',
                    extension: '.png',
                    text: 'DIGITAL COMICS'
                },
                {
                    url: 'buy-comics',
                    path: '-merchandise',
                    extension: '.png',
                    text: ' DCMERCHANDISE'
                },
                {
                    url: 'buy-comics',
                    path: '-subscriptions',
                    extension: '.png',
                    text: 'SUBSCRIPTIONS'
                },
                {
                    url: 'buy-comics',
                    path: '-shop-locator',
                    extension: '.png',
                    text: 'COMIC SHOP LOCATOR'
                },
                {
                    url: 'buy-dc',
                    path: '-power-visa',
                    extension: '.svg',
                    text: 'POWER VISA'
                }
            ],
            cards: cards
      }
    }
}
</script>

<style scoped lang="scss">
@import "../style/mood";
@import "../style/mixing";

.main-top {
    @include center(vertical);
    width: 100%;
    height: 680px;
    background-color: $dark;
    color: $light;


    .icon-main {
        display: flex;
        flex-wrap: wrap;
        width: 70%;
        height: 100%;
        font-size: 20px;
        margin: 0 auto;
        


        .icon {
            display: flex;
            flex-direction: column;
            align-items: center;
            width: calc(100% / 6);

            img {
                height: 210px;
                width: 200px;

            }
        }
    }
}

.main-bott {
    @include center(vertical);
    justify-content: center;
    width: 100%;
    height: 140px;
    background-color: $primary;

    ul {
        @include center(vertical);
        justify-content: space-around;
        list-style: none;
        margin: 0 auto;
        width: 65%;

        li {
            @include center(vertical);
            justify-content: center;
            width: 12%;
            color: $light;

            span {
                font-size: 12px;
                margin-left: 8px;
            }
        }
    }

    img {
        max-width: 45px;
        max-height: 45px;
    }
}
</style>

