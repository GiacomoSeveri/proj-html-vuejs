<script>
import GamerLogo from './GamerLogo.vue';
import SectionText from './SectionText.vue';
import SocialImg from './SocialImg.vue';
export default {
    name: 'GameColumn',
    components: { GamerLogo, SectionText, SocialImg },
    data() {
        return {
            text: 'Upropriate brand economca sound technolog after covalent technology enable prospective wastng markets whereas propriate and brand economca sound technolog'
        }
    }
}
</script>

<template>
    <div class="d-flex flex-column ciao px-2">
        <gamer-logo></gamer-logo>
        <section-text :text="text"></section-text>
        <social-img></social-img>
    </div>
</template>

<style lang="scss" scoped>
.ciao {
    width: 33%;
}
</style>