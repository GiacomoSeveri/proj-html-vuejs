<script>
import Title from '../../utilities/Title.vue';
import SectionTitle from '../../utilities/SectionTitle.vue';
import TeamCard from '../../utilities/TeamCard.vue';
import ComunityCard from '../../utilities/ComunityCard.vue';
export default {
    name: 'AnySection',
    components: { Title, SectionTitle, TeamCard, ComunityCard },
    data() {
        return {
            section: 'OUR TEAM PLAYERS',
            title: 'MEET OUR SQUAD PLAYERS',
            items: [
                { name: 'GAMING TEAM', img: '-2' },
                { name: 'DRAGON TEAM', img: 'sm-1' },
                { name: 'FROGS TEAM', img: 'sm-3' },
                { name: 'MONKAY TEAM', img: 'sm-12' },
                { name: 'SHARK TEAM', img: 'sm-5' }
            ],

        }
    }
}
</script>

<template>
    <section-title :section="section"></section-title>
    <Title :title="title"></Title>
    <team-card :items="items"></team-card>
    <comunity-card></comunity-card>
</template>

<style lang="scss" scoped>

</style>