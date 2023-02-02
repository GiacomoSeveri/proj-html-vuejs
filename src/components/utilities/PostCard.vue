<script>
import SectionText from './SectionText.vue';

export default {
    name: 'ShopCard',
    props: { items: Array },
    components: { SectionText },
    data() {
        return {
            text: 'Distinctively provide acces mutfuncto user whereas transparent proceses omes ncentivize functionalities than an extensible archtectur services and cross, Distinctively provide acces mutfuncto user whereas transparent proceses omes ncentivize functionalities than an extensible archtectur services and cross'
        }
    }
}
</script>

<template>
    <div class="d-flex">
        <div v-for="item in items" class="mx-3 my-4 custom-card">
            <div class="d-flex justify-content-between">
                <img :src="`imgs/${item.img}.jpg`" alt="">
                <div class="text-start">
                    <p class="m-0">{{ item.name }}</p>
                    <span>{{ item.role }}</span>
                </div>
                <img :src="`imgs/${item.log}.png`" alt="">
            </div>
            <div>
                <hr>
                <section-text :text="text" class="text-start"></section-text>
                <i v-for="n in 5" class="fa-regular fa-star my-2 mx-1 text-start i"></i>
                <span class="text-start i ms-2">{{ item.vote }}</span>

            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.custom-card {
    background-color: #232a5c;
    padding: 15px;

    img {
        cursor: pointer;
        width: 50px;
        // border: solid 10px #232a5c;
    }

    .i {
        cursor: pointer;
        color: #00b67a;
    }
}
</style>