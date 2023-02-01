<script>
import Title from '../../utilities/Title.vue';
import SectionTitle from '../../utilities/SectionTitle.vue';
import NowMatch from '../../utilities/NowMatch.vue';
import WhiteButton from '../../utilities/WhiteButton.vue';
import NextMatch from '../../utilities/NextMatch.vue'
export default {
    name: 'AnySection',
    components: { Title, SectionTitle, NowMatch, WhiteButton, NextMatch },
    data() {
        return {
            section: 'ANYWHERE, ANYTIME',
            title: 'ALL MATCHES SCHEDULE',
            items: [
                { group: '2 GROUP 32 PLAYERS', pool: 'PRIZE POOL $3200', res: '', torn: 'BATTELFIELD-4 TOURNAMENT', info: '30 APR 2022 / Time 08:30PM', team1: 'sm-6', team2: 'sm-9' },
            ],
            textWhite: 'BROWSE ALL MATCHES',
            details: [
                { group: '2 GROUP 32 PLAYERS', pool: 'PRIZE POOL $3200', res: '', torn: 'CALL OF DUTY TOURNAMENT', info: '30 APR 2022 / Time 08:30PM', team1: 'sm-1', team2: 'sm-2' },
                { group: '2 GROUP 32 PLAYERS', pool: 'PRIZE POOL $3200', res: '4 - 2', torn: '', info: '30 APR 2022 / Time 08:30PM', team1: 'sm-7', team2: 'sm-8' },
                { group: '2 GROUP 32 PLAYERS', pool: 'PRIZE POOL $3200', res: '', torn: 'LEAGUE BATTLE TOURNAMENT', info: '30 APR 2022 / Time 08:30PM', team1: 'sm-3', team2: 'sm-4' },
                { group: '2 GROUP 32 PLAYERS', pool: 'PRIZE POOL $3200', res: '8 - 4', torn: '', info: '30 APR 2022 / Time 08:30PM', team1: 'sm-9', team2: 'sm-10' },
                { group: '2 GROUP 32 PLAYERS', pool: 'PRIZE POOL $3200', res: '', torn: 'PUBG CLASSIC TOURNAMENT', info: '30 APR 2022 / Time 08:30PM', team1: 'sm-5', team2: 'sm-6' },
                { group: '2 GROUP 32 PLAYERS', pool: 'PRIZE POOL $3200', res: '3 - 4', torn: '', info: '30 APR 2022 / Time 08:30PM', team1: 'sm-11', team2: 'sm-12' },
            ]
        }
    }
}
</script>

<template>
    <section-title :section="section"></section-title>
    <Title :title="title"></Title>
    <now-match class="mb-5" :items="items"></now-match>
    <next-match class="mb-5" :details="details"></next-match>
    <white-button :textWhite="textWhite"></white-button>

</template>

<style lang="scss" scoped>

</style>