<script>
import SectionTitle from '../../utilities/SectionTitle.vue';
import Title from '../../utilities/Title.vue';
import Video from '../../utilities/Video.vue';
export default {
    name: 'VideoSection',
    components: { SectionTitle, Title, Video },
    data() {
        return {
            section: 'OUR LATEST VIDEOS',
            title: 'CHACK OUR LIVE STREAMING'
        }
    }
}
</script>

<template>
    <section-title :section="section"></section-title>
    <Title :title="title"></Title>
    <Video></Video>
</template>

<style>

</style>