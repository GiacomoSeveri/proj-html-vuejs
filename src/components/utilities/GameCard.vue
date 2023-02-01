<script>
export default {
    name: 'GameCard',
    data() {
        return {

        }
    }
}
</script>

<template>
    <div class="d-flex justify-content-center align-items-center">
        <div class="custom-card d-flex justify-content-center align-items-center">
            <img src="imgs/team-1.png" alt="">
            <img src="imgs/vs.png" alt="" class="vs mx-4">
            <img src="imgs/team-2.png" alt="">
        </div>
        <div class="custom-card d-flex justify-content-center align-items-center">
            <img src="imgs/teamsm-4.png" alt="">
            <img src="imgs/vs.png" alt="" class="vs mx-4">
            <img src="imgs/teamsm-3.png" alt="">
        </div>
        <div class="custom-card d-flex justify-content-center align-items-center">
            <img src="imgs/teamsm-2.png" alt="">
            <img src="imgs/vs.png" alt="" class="vs mx-4">
            <img src="imgs/teamsm-1.png" alt="">
        </div>
    </div>
</template>

<style lang="scss" scoped>
.custom-card {
    height: 180px;
    width: 300px;
    background-color: #232A5C;
    border: solid 1px #ff0052;
    border-radius: 5px;
    cursor: pointer;
    margin: 50px;
}

img {
    width: auto;
    height: 90px;
    object-fit: fill;
}

.vs {
    width: 30px;
    height: 30px;
    margin: 0 10px;
}
</style>