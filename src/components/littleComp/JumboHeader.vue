<script>
import WhiteButton from '../utilities/WhiteButton.vue';
import Subtitle from '../utilities/subtitle.vue';
import SectionText from '../utilities/SectionText.vue';
export default {
    name: 'JamboHeader',
    components: { WhiteButton, Subtitle, SectionText },
    data() {
        return {
            textWhite: 'JOIN US TODAY',
            title: 'GENUINE MONEY TRANSACTION',
            text: 'Assertively Communicate An Expanded Array Of Mindshare Rather Than Diverse Technologies For Magnetic Applications Eamlessly Virtual Then Conveniently Monetize Synergistic Human Capital'
        }
    }

}
</script>

<template>
    <div class="ciao">
        <h1 class="my-3">ONLINE GAME</h1>
        <subtitle class="my-3" :title="title"></subtitle>
        <section-text :text="text"></section-text>
        <white-button class="my-3" :textWhite="textWhite"></white-button>
    </div>
</template>

<style lang="scss" scoped>
.ciao {
    margin: 130px 0;
    width: 50%;

    h1 {
        font-weight: 700;
    }
}
</style>