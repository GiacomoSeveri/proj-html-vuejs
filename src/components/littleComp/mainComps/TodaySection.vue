<script>
import Title from '../../utilities/Title.vue';
import SectionTitle from '../../utilities/SectionTitle.vue';
import WhiteButton from '../../utilities/WhiteButton.vue';
import GameCard from '../../utilities/GameCard.vue';
export default {
    name: 'TodaySection',
    components: { Title, SectionTitle, WhiteButton, GameCard },
    data() {
        return {
            section: 'TODAY`S',
            title: 'OUR GAME COLLECTION',
            textWhite: 'BROWSE ALL GAME'
        }
    }
}
</script>

<template>
    <section-title :section="section"></section-title>
    <Title :title="title"></Title>
    <game-card></game-card>
    <white-button :textWhite="textWhite"></white-button>
    <hr>
</template>

<style lang="scss" scoped>
hr {
    color: #fff;
    width: 50%;
    margin: 45px 350px;
}
</style>