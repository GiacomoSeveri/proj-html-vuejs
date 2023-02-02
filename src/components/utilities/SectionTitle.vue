<script>
export default {
    name: 'SectionTitle',
    props: { section: String }
}
</script>

<template>
    <h3>{{ section }}</h3>
</template>

<style lang="scss" scoped>
h3 {
    font-size: 15px;
    font-weight: 700;
    color: #5F0F40;
}
</style>