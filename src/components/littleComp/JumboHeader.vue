<script>
import WhiteButton from '../utilities/WhiteButton.vue';
import Subtitle from '../utilities/subtitle.vue';
export default {
    name: 'JamboHeader',
    components: { WhiteButton, Subtitle },
    data() {
        return {
            textWhite: 'JOIN US TODAY',
            title: 'GENUINE MONEY TRANSACTION'
        }
    }

}
</script>

<template>
    <h1>ONLINE GAME</h1>
    <subtitle :title="title"></subtitle>
    <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Inventore repellendus, ut porro, recusandae totam
        facere aspernatur non a veritatis deleniti saepe adipisci eligendi vero aperiam amet magnam libero vel harum.
    </p>
    <white-button :textWhite="textWhite"></white-button>
</template>

<style lang="scss" scoped>

</style>