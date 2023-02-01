<script>
import Title from '../../utilities/Title.vue';
import SectionTitle from '../../utilities/SectionTitle.vue';
import SectionText from '../../utilities/SectionText.vue';
import WhoCard from '../../utilities/WhoCard.vue'
export default {
    name: 'TodaySection',
    components: { Title, SectionTitle, SectionText, WhoCard },
    data() {
        return {
            section: 'WHO WE ARE',
            title: 'WE ARE PROFESSIONAL TEAM ESPORT',
            text: 'Distinctively provide acces mutfuncto user whereas transparent proceses omes ncentivize functionalities than an extensible archtectur services and cross',
            items: [
                { title: '100K COMUNITY EARNING', text: 'Distinctively provide acces mutfuncto user whereas communicate leveraged services', img: 'icon-1' },
                { title: '34M+ REGISTERED PLAYER', text: 'Distinctively provide acces mutfuncto user whereas communicate leveraged services', img: 'icon-2' },
                { title: '240K STREAMING COMPLETE', text: 'Distinctively provide acces mutfuncto user whereas communicate leveraged services', img: 'icon-3' },
            ]
        }
    }
}
</script>

<template>
    <div class="d-flex justify-content-center align-items-center">
        <img src="imgs/01.png" alt="">
        <div class="ms-4">
            <section-title :section="section"></section-title>
            <Title :title="title"></Title>
            <section-text :text="text"></section-text>
            <who-card :items="items"></who-card>
        </div>
    </div>
</template>

<style lang="scss" scoped>
img {
    max-width: 500px;
}
</style>