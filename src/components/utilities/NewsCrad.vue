<script>
import SectionText from './SectionText.vue';
import PinkButton from './PinkButton.vue';
export default {
    name: 'NewsCard',
    props: { items: Array },
    components: { SectionText, PinkButton },
    data() {
        return {
            text: 'Distinctively provide acces mutfuncto user whereas transparent proceses omes ncentivize functionalities than an extensible archtectur services and cross, istinctively provide acces mutfuncto user whereas transparent proceses omes ncentivize functionalities than an extensible archtectur services and cross',
            textPink: 'READ MORE'
        }
    }
}
</script>

<template>
    <div class="d-flex justify-content-center align-items-center mt-5 text-start">
        <div v-for="item in items" class="mx-2 custom-card">
            <img :src="`imgs/${item.img}.jpg`" class="mb-3">
            <h5>{{ item.title }}</h5>
            <p class="my-2 fw-bold text-secondary">{{ item.data }}</p>
            <section-text :text="text"></section-text>
            <pink-button :textPink="textPink" class="mb-2"></pink-button>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.custom-card {
    background-color: rgb(35, 42, 92, 0.8);
    padding: 6px;

    img {
        cursor: pointer;
        width: 100%;
        border: solid 10px rgb(35, 42, 92, 0.6);
    }

    p {
        font-size: 12px;
    }
}
</style>