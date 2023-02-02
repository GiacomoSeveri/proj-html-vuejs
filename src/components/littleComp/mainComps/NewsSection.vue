<script>
import SectionTitle from '../../utilities/SectionTitle.vue'
import Title from '../../utilities/Title.vue';
import NewsCard from '../../utilities/NewsCrad.vue'
export default {
    mane: 'NewsSection',
    components: { SectionTitle, Title, NewsCard },
    data() {
        return {
            section: 'OUR RECENT NEWS',
            title: 'OUR MOST POPULAR BLOG POSTS',
            items: [
                { img: '01 (3)', data: 'Admin / 01 January 2022', title: 'DISTINCTIVE REDEFINE RESOURCE MIXIMIZING FOR' },
                { img: '02 (4)', data: 'Admin / 01 January 2022', title: 'REDEFINE RESOURCE MIXIMIZING FOR DISTINCTIVE' }
            ]
        }
    }
}
</script>

<template>
    <section-title :section="section"></section-title>
    <Title :title="title"></Title>
    <news-card :items="items"></news-card>
</template>

<style>

</style>