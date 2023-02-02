<script>

export default {
    name: 'ShopCard',
    props: { items: Array },

}
</script>

<template>
    <div class="d-flex justify-content-center align-items-center mt-5">
        <div v-for="item in items" class="mx-3 custom-card">
            <img :src="`imgs/${item.img}.jpg`" class="mb-3">
            <p class="m-0 fw-bold">{{ item.name }}</p>
            <p class="m-0 fw-bold">{{ item.price }}</p>
            <i v-for="n in 5" class="fa-solid fa-star my-2 mx-1"></i>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.custom-card {
    background-color: #232a5c;

    img {
        cursor: pointer;
        width: 220px;
        border: solid 10px #232a5c;
    }

    i {
        cursor: pointer;
    }

    &:hover {
        background-color: #5F0F40;

        img {
            border: solid 10px #5F0F40;

        }
    }
}
</style>