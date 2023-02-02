<script>
export default {
    name: 'FooterList',
    props: { items: Array }
}
</script>

<template>
    <div v-for="item in items">
        <img :src="`imgs/${item.icon}.png`" alt="">

    </div>
</template>