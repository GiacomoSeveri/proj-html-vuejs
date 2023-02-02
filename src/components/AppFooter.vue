<script>
import InfoFooter from './littleComp/footerComps/InfoFooter.vue';
import MainFooter from './littleComp/footerComps/MainFooter.vue'
import LastElement from './littleComp/footerComps/LastElement.vue';
export default {
    name: 'AppFooter',
    components: { InfoFooter, MainFooter, LastElement }
}
</script>

<template>
    <div class="custom-bgi">
        <div class="container">
            <info-footer></info-footer>
            <main-footer></main-footer>
        </div>
    </div>
    <last-element></last-element>


</template>

<style lang="scss" scoped>
.custom-bgi {
    background-image: url('imgs/bg (3).jpg');
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    // height: 300vh;
    padding: 3rem;
}
</style>