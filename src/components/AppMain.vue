<script>
import TodaySection from './littleComp/mainComps/TodaySection.vue'
import WhoSection from './littleComp/mainComps/WhoSection.vue'
export default {
    name: 'AppMain',
    components: { TodaySection, WhoSection }
}
</script>

<template>
    <section id="today" class="text-center">
        <today-section></today-section>
    </section>
    <section id="who">
        <div class="custom-mis">
            <who-section></who-section>
        </div>
    </section>
    section#
</template>

<style lang="scss" scoped>
#today {
    background-color: #131661;
    height: 75vh;
    padding: 3.5rem;
}

#who {
    background-color: #131661;
    height: 90vh;
    padding: 3.5rem;
}

.custom-mis {
    max-width: 1140px;
    margin: 0 auto;
}
</style>