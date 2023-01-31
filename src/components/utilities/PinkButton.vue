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
    background-color: #ff0052;

    &:hover {
        color: #000;
        background-color: #e20048;
    }
}
</style>