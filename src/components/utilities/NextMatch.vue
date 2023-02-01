<script>
import Social from './SocialImg.vue';
export default {
    name: 'NextMatch',
    components: { Social },
    props: { details: Array },

    data() {
        return {
        }
    }
}
</script>

<template>
    <div class="row d-flex justify-content-center">
        <div class="col-4 mt-4 mx-3 d-flex justify-content-between flex-column" v-for="item in details">
            <div class="info p-1 d-flex justify-content-between">
                <span>{{ item.group }}</span>
                <span>{{ item.pool }}</span>
            </div>
            <div class="m-0 p-1 d-flex justify-content-between bgc-custom">
                <img :src="`imgs/team${item.team1}.png`" class="mx-2">
                <div>
                    <p class="m-0">{{ item.torn }}</p>
                    <p class="m-0">{{ item.res }}</p>
                    <span class="text-secondary">{{ item.info }}</span>
                    <social></social>
                </div>
                <img :src="`imgs/team${item.team2}.png`" class="mx-2">

            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.info {
    background-color: #ff0052;
}

.bgc-custom {
    background-color: #fff;
}

p {
    font-size: 20px;
    font-weight: 500;
    color: #000;
}

span {
    font-size: 11px;
}

img {
    max-width: 55px;
    cursor: pointer;
    object-fit: contain;
}
</style>