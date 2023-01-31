<script>
export default {
    name: 'SectionText',
    props: { text: String }
}
</script>

<template>
    <p>{{ text }}</p>
</template>

<style lang="scss" scoped>
p {
    font-size: 16px;
    line-height: 20px;
}
</style>