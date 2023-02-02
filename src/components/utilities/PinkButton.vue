<script>
export default {
    name: 'PinkButton',
    props: { textPink: String }
}
</script>

<template>
    <button type="button" class="btn">{{ textPink }}</button>

</template>

<style lang="scss" scoped>
button {
    color: #fff;
    box-shadow: #fff 2px 3px;
    font-weight: 700;
    background-color: #5F0F40;

    &:hover {
        color: #fff;
        background-color: #ff0052;
    }
}
</style>