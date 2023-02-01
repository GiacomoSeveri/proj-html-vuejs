<script>
import TodaySection from './littleComp/mainComps/TodaySection.vue'
export default {
    name: 'AppMain',
    components: { TodaySection }
}
</script>

<template>
    <section id="today" class="text-center">
        <today-section></today-section>
    </section>
</template>

<style lang="scss" scoped>
#today {
    background-color: #131661;
    height: 65vh;
    padding: 3.5rem;
}
</style>