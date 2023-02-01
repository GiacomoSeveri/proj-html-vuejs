<script>
import GamerLogo from '../../utilities/GamerLogo.vue';
import WhiteButton from '../../utilities/WhiteButton.vue';
import PinkButton from '../../utilities/PinkButton.vue';
export default {
    name: 'MainHeader',
    components: { GamerLogo, WhiteButton, PinkButton },
    data() {
        return {
            voice: [
                { url: '#', text: 'HOME' },
                { url: '#', text: 'FEATURES +' },
                { url: '#', text: 'ACHIEVEMENT' },
                { url: '#', text: 'BLOG+' },
                { url: '#', text: 'CONTACT' },
            ],
            textWhite: 'LOG IN',
            textPink: 'SING UP'
        }
    }
}
</script>

<template>
    <div class="d-flex justify-content-between align-items-center">
        <gamer-logo></gamer-logo>
        <ul class="d-flex justify-content-between align-items-center">
            <a v-for="option in voice" href="{{ option.url }}">
                <li>{{ option.text }}</li>
            </a>
            <li>
                <white-button :textWhite="textWhite" class="py-2 px-3 me-1"></white-button>
                <pink-button :textPink="textPink" class="py-2 px-3"></pink-button>
            </li>
        </ul>
    </div>
</template>

<style lang="scss" scoped>
ul {
    list-style-type: none;

    a {
        color: #fff;
        text-decoration: none;

        li {
            padding: 0 15px;
            font-size: 15px;
            cursor: pointer;
        }
    }
}
</style>