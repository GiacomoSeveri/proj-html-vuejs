<script>
import SectionTitle from '../../utilities/SectionTitle.vue'
import Title from '../../utilities/Title.vue'
import PostCard from '../../utilities/PostCard.vue'
export default {
    name: 'TestimonialsSection',
    components: { SectionTitle, Title, PostCard },
    data() {
        return {
            section: 'OUR RECENT NEWS',
            title: 'OUR MOST POPULAR TESTIMONIALS POSTS',
            items: [
                { img: '01 (2)', name: 'MADLEY PONDOR', role: 'UI Designer', log: '08', vote: '5.28' },
                { img: '02 (2)', name: 'OLIVER BEDDOWS', role: 'UI Designer', log: '06', vote: '5.28' },
            ]
        }
    }
}
</script>

<template>
    <section-title :section="section"></section-title>
    <Title :title="title"></Title>
    <post-card :items="items"></post-card>
</template>

<style lang="scss" scoped>
hr {
    color: #fff;
    width: 50%;
    margin: 45px 350px;
}
</style>