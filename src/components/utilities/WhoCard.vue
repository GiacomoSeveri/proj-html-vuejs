<script>
export default {
    name: 'WhoCard',
    props: { items: Array }

}
</script>

<template>
    <div v-for="(item, i) in items" class="d-flex mb-3">
        <img :src="`imgs/${item.img}.png`" alt="">
        <div>
            <h5 class="m-0">{{ item.title }}</h5>
            <span>{{ item.text }}</span>
        </div>
    </div>
</template>

<style lang="scss" scoped>
img {
    background-color: #ff0052;
    padding: 10px;
    border-radius: 50%;
    width: 50px;
    height: 50px;
    margin: 0 7px;
    cursor: pointer;
}
</style>