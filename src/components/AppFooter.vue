<script>
import InfoFooter from './littleComp/footerComps/InfoFooter.vue';
export default {
    name: 'AppFooter',
    components: { InfoFooter }
}
</script>

<template>
    <div class="custom-bgi">
        <div class="container">
            <info-footer></info-footer>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.custom-bgi {
    background-image: url('imgs/bg (3).jpg');
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    height: 100vh;
    padding: 3rem;
}
</style>