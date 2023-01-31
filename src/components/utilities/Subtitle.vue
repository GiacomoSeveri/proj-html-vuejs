<script>
export default {
    name: 'Subtitle',
    props: { title: String }
}
</script>

<template>
    <h3>{{ title }}</h3>
</template>

<style lang="scss" scoped>
h3 {
    font-size: 15px;
    font-weight: 600;
}
</style>