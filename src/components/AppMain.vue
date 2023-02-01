<script>
import TodaySection from './littleComp/mainComps/TodaySection.vue'
import WhoSection from './littleComp/mainComps/WhoSection.vue'
import AnySection from './littleComp/mainComps/AnySection.vue'
export default {
    name: 'AppMain',
    components: { TodaySection, WhoSection, AnySection }
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
    <section id="any" class="text-center">
        <any-section></any-section>
    </section>
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

    .custom-mis {
        max-width: 1140px;
        margin: 0 auto;
    }
}

#any {
    background-image: url('imgs/bg (1).jpg');
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    height: 115vh;
    padding: 3.5rem;

}
</style>