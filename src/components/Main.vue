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
