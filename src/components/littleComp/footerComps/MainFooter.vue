<script>
import GameColumn from '../../utilities/GameColumn.vue';
import PokerColumn from '../../utilities/PokerColumn.vue'
import LetterColumn from '../../utilities/LetterColumn.vue';
export default {
    name: 'MainFooter',
    components: { GameColumn, PokerColumn, LetterColumn }
}
</script>

<template>
    <div class="custom-mis d-flex justify-content-center">
        <!-- <game-column></game-column> -->
        <!-- <game-column></game-column> -->
        <game-column></game-column>
        <poker-column></poker-column>
        <letter-column></letter-column>
    </div>
</template>

<style lang="scss" scoped>
.custom-mis {
    padding: 3rem;
}
</style>