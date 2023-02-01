<script>
export default {
    name: 'Subtitle',
    props: { title: String }
}
</script>

<template>
    <h2>{{ title }}</h2>
</template>

<style lang="scss" scoped>
h2 {
    font-size: 25px;
    font-weight: 700;
}
</style>