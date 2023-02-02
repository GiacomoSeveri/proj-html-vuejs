<script>
import SectionTitle from '../../utilities/SectionTitle.vue'
import Title from '../../utilities/Title.vue'
import ShopCard from '../../utilities/ShopCard.vue'
export default {
    name: 'ShopSection',
    components: { SectionTitle, Title, ShopCard },
    data() {
        return {
            section: 'GAMER T-SHIRT`S',
            title: 'EXPLORE OUR PRODUCTS',
            items: [
                { img: '01 (1)', name: 'BLACK T-SHIRT HERE', price: '$380.00' },
                { img: '02 (1)', name: 'GREEN T-SHIRT HERE', price: '$380.00' },
                { img: '03 (2)', name: 'YELLOW T-SHIRT HERE', price: '$380.00' },
                { img: '04 (1)', name: 'BLUE T-SHIRT HERE', price: '$380.00' }
            ]
        }
    }
}
</script>

<template>
    <section-title :section="section"></section-title>
    <Title :title="title"></Title>
    <shop-card :items="items"></shop-card>
    <hr>
</template>

<style lang="scss" scoped>
hr {
    color: #fff;
    width: 50%;
    margin: 45px 350px;
}
</style>