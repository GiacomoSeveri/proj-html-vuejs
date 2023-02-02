<script>
export default {
    name: 'PartnerCard',
    props: { items: Array },
}
</script>

<template>
    <div class="col-5 container my-3">
        <img v-for="item in items" :src="`imgs/${item.img}.png`" class="mx-3 my-4">
    </div>
</template>

<style lang="scss" scoped>
img {
    width: 80px;
    cursor: pointer;
    // margin: 1rem;
}
</style>