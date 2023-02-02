<script>
import TitleVue from './Title.vue';
import PokerCard from './PokerCard.vue';
export default {
    name: 'PokerColumn',
    components: { TitleVue, PokerCard },
    data() {
        return {
            title: 'TOP JACKPOT GAMES',
            items: [
                { img: '01 (4)', name: 'FREE POKER GAME', poker: '$230' },
                { img: '02 (3)', name: 'CLUB POKER GAME', poker: '$290' },
                { img: '03', name: 'ROYAL POKER GAME', poker: '$330' },
            ]
        }
    }
}
</script>

<template>
    <div class="d-flex flex-column">
        <title-vue :title="title"></title-vue>
        <poker-card :items="items"></poker-card>
    </div>
</template>

<style>

</style>