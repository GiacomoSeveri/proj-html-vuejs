<script>
export default {
    name: 'PokerCard',
    props: { items: Array }
}
</script>

<template>
    <div v-for="item in items" class="d-flex">
        <img :src="`imgs/${item.img}.jpg`" class="me-2 mb-2">
        <div>
            <p class="m-0">{{ item.name }}</p>
            <span>Poker <strong>{{ item.poker }}</strong></span>
        </div>
    </div>
</template>

<style lang="scss" scoped>

</style>