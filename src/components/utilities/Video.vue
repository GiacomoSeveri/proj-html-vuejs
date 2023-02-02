<script>
import CoverImgMain from './CoverImgMain.vue'
import CoverImgSec from './CoverImgSec.vue'
export default {
    name: 'Video',
    components: { CoverImgMain, CoverImgSec },
    data() {
        return {
            main: [
                { img: '01 (3)', text: '2022 LVP SUPERLIGA ORANGE SUMMER', url: '#' },
                { img: '02', text: 'PUBG CLASSIC TOURNAMENT', url: '#' }
            ],
            sec: [
                { img: '03 (1)', text: 'CAN I ADD MY LOCAL BANK...', url: '#' },
                { img: '04', text: 'LEAGUE BATTLE TOURNAMENT.', url: '#' },
                { img: '05', text: 'WHERE CAN I REDEEM MY...', url: '#' },
            ]
        }
    }
}
</script>

<template>
    <cover-img-main :main="main"></cover-img-main>
    <cover-img-sec :sec="sec"></cover-img-sec>
</template>

<style>

</style>