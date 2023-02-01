<script>
import SocialImg from './SocialImg.vue';
export default {
    name: 'TeamCard',
    components: { SocialImg },
    props: { items: Array },

}
</script>

<template>
    <div class="d-flex justify-content-center align-items-center mt-5">
        <figure v-for="item in items"
            class="mx-2 d-flex justify-content-center align-items-center flex-column custom-bgc">
            <img :src="`imgs/team${item.img}.png`" alt="{{ item.name }}" class="my-3">
            <h4 class="my-3">{{ item.name }}</h4>
            <social-img class="my-3"></social-img>
        </figure>
    </div>
</template>

<style lang="scss" scoped>
.custom-bgc {
    background-image: url('imgs/5.jpg');
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    padding: 1rem;
    width: calc(100% / 5);
    height: 55vh;
    border: solid 10px #131661;

    img {
        max-width: 300px;
        cursor: pointer;
    }
}
</style>