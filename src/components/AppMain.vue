<script>
import TodaySection from './littleComp/mainComps/TodaySection.vue'
import WhoSection from './littleComp/mainComps/WhoSection.vue'
import AnySection from './littleComp/mainComps/AnySection.vue'
import TeamSection from './littleComp/mainComps/TeamSection.vue'
import VideoSection from './littleComp/mainComps/VideoSection.vue'
import ShopSection from './littleComp/mainComps/ShopSection.vue'
export default {
    name: 'AppMain',
    components: { TodaySection, WhoSection, AnySection, TeamSection, VideoSection, ShopSection }
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
    <section id="team" class="text-center">
        <team-section></team-section>
    </section>
    <section id="video" class="text-center">
        <video-section></video-section>
    </section>
    <section id="shop" class="text-center">
        <shop-section></shop-section>
    </section>
</template>

<style lang="scss" scoped>
#today {
    background-color: #131661;
    padding: 3.5rem;
}

#who {
    background-color: #131661;
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
    padding: 3.5rem;
}

#team {
    background-color: #131661;
    padding: 3.5rem;
}

#video {
    background-image: url('imgs/bg (3).jpg');
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    padding: 3.5rem;
}

#shop {
    background-color: #131661;
    padding: 3.5rem;
    height: 150vh;
}
</style>