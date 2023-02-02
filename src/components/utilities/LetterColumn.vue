<script>
import TitleVue from './Title.vue';
import SectionText from './SectionText.vue';
import WhiteButton from './WhiteButton.vue';
export default {
    name: 'LetterColumn',
    components: { TitleVue, SectionText, WhiteButton },
    data() {
        return {
            title: 'OUR NEWSLETTER',
            text: 'Gamer esports organization supported by community leaders',
            textWhite: 'SEND MESSAGE'
        }
    }
}
</script>

<template>
    <div class="d-flex flex-column ciao">
        <title-vue :title="title"></title-vue>
        <section-text :text="text"></section-text>
        <div class="mb-3">
            <input type="name" class="form-control bgc-custom" placeholder="YOUR NAME">
        </div>
        <div class="mb-3">
            <input type="email" class="form-control bgc-custom" placeholder="YOUR EMAIL">
        </div>
        <white-button :textWhite="textWhite"></white-button>
    </div>
</template>

<style lang="scss" scoped>
.ciao {
    padding: 0px 3rem;

    .bgc-custom {
        background-color: #232a5c;
        color: #fff;
    }
}
</style>