<script>
import PinkButton from './PinkButton.vue';
import Social from './SocialImg.vue';
export default {
    name: 'NowMatch',
    components: { PinkButton, Social },
    props: { items: Array },

    data() {
        return {
            textPink: 'WATCH NOW'
        }
    }
}
</script>

<template>
    <div class="row d-flex justify-content-center">
        <div class="col-8 mt-4 d-flex justify-content-between info" v-for="item in items">
            <span>{{ item.group }}</span>
            <span>{{ item.pool }}</span>
        </div>
        <div class="col-8 m-0 d-flex justify-content-between align-items-center scheduls" v-for="item in items">
            <div>
                <p class="m-0">{{ item.torn }}</p>
                <span class="text-secondary">{{ item.info }}</span>
            </div>
            <figure class="m-0">
                <img :src="`imgs/team${item.team1}.png`">
                <img src="imgs/vs.png" alt="" class="vs mx-4">
                <img :src="`imgs/team${item.team2}.png`">
            </figure>
            <div class="d-flex justify-content-center align-items-center">
                <social></social>
                <pink-button :textPink="textPink"></pink-button>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.info {
    background-color: #ff0052;
}

.scheduls {
    background-color: #fff;
    color: #000;
    padding: 5px;

    p {
        font-size: 13px;
        font-weight: 500;
    }

    span {
        font-size: 11px;
    }

    img {
        max-width: 55px;
        cursor: pointer;
        object-fit: contain;
    }
}
</style>