<script>
import WhiteButton from './WhiteButton.vue';
import SectionTitle from './SectionTitle.vue';
import Subtitle from './Title.vue';
import SectionText from './SectionText.vue';
export default {
    name: 'ComunityCard',
    components: { WhiteButton, Subtitle, SectionText, SectionTitle },
    data() {
        return {
            section: 'LET`S PLAY TOGETHER',
            textWhite: 'JOIN COMUNITY',
            title: 'JOIN GAMER ESPORTS TO BECOME NEXT PRO GAMER TODAY!',
            text: 'Distinctively provide acces mutfuncto user whereas transparent proceses omes ncentivize functionalities than an extensible archtectur services and cross'
        }
    }

}
</script>

<template>
    <div class="comunity-card text-start d-flex mt-5">
        <div>
            <section-title :section="section"></section-title>
            <subtitle class="my-3" :title="title"></subtitle>
            <section-text :text="text"></section-text>
            <white-button class="my-3" :textWhite="textWhite"></white-button>
        </div>
        <img src="imgs/01 (1).png" alt="01 (1).png">
    </div>
</template>

<style lang="scss" scoped>
.comunity-card {
    width: 60%;
    height: auto;
    margin: 0 auto;
    background-image: url('imgs/bg (4).jpg');
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    padding: 2rem;
    border: solid 1px #ff0052;
}

img {
    max-width: 350px;
}
</style>