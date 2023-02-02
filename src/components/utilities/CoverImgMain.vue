<script>
import PinkButton from './PinkButton.vue';
export default {
    name: 'CoverImgMain',
    components: { PinkButton },
    props: { main: Array },
    data() {
        return {
            textPink: 'WATCH NOW'
        }
    }
}
</script>

<template>
    <div class="d-flex justify-content-center align-items-center">
        <div v-for="data in main" class="father">
            <img :src="`imgs/${data.img}.jpg`" class="mt-5 mx-2">
            <div class="play">
                <a href="{{ data.url }}"><i class="fa-solid fa-play"></i> </a>
            </div>
            <div class="son d-flex justify-content-start align-items-start flex-column">
                <pink-button :textPink="textPink" class="mb-2"></pink-button>
                <span>{{ data.text }}</span>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.father {
    position: relative;
}

.play {
    font-size: 55px;

    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);

    a {
        text-decoration: none;
        color: #5F0F40;

        &:hover {
            color: #ff0052;
        }
    }
}

.son {
    position: absolute;
    bottom: 10px;
    left: 30px;
}

img {
    width: 500px;
    // height: 300px;
    object-fit: contain;
    border: solid 7px #232a5c;
}
</style>