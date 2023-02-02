<script>
import SectionTitle from '../../utilities/SectionTitle.vue'
import Title from '../../utilities/Title.vue';
import PartnerCard from '../../utilities/PartnerCard.vue'
import WhiteButton from '../../utilities/WhiteButton.vue';
export default {
    mane: 'PartnerSection',
    components: { SectionTitle, Title, PartnerCard, WhiteButton },
    data() {
        return {
            section: 'WE OUR PARTNERS',
            title: 'BECOME A PARTNER OF GAMER',
            items: [
                { img: '01 (2)' },
                { img: '01 (3)' },
                { img: '06' },
                { img: '07' },
                { img: '05' },
                { img: '06' },
                { img: '01 (2)' },
                { img: '01 (3)' }
            ],
            textWhite: 'BECOME A PARTNER'
        }
    }
}
</script>

<template>
    <section-title :section="section"></section-title>
    <Title :title="title"></Title>
    <partner-card :items="items"></partner-card>
    <white-button :textWhite="textWhite"></white-button>
</template>

<style>

</style>