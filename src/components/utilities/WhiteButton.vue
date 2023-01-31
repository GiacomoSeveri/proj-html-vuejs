<script>
export default {
    name: 'WhiteButton',
    props: { textWhite: String }
}
</script>

<template>
    <button type="button" class="btn btn-light">{{ textWhite }}</button>
</template>

<style lang="scss" scoped>
button {
    color: #ff0052;
    box-shadow: #ff0052 2px 3px;
    font-weight: 700;
}
</style>