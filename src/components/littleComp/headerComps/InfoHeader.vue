<script>
export default {
    name: 'InfoHeader',
    data() {
        return {

        }
    }
}
</script>

<template>
    <div class="d-flex justify-content-between">
        <ul class="d-flex justify-content-between">
            <li>
                <a href="#">
                    <i class="fa-solid fa-phone"></i>
                    <span>+800-123-4567 6587</span>
                </a>
            </li>
            <li>
                <a href="#">
                    <i class="fa-solid fa-location-dot"></i>
                    <span>Beaverly, New York 224 USA</span>
                </a>
            </li>
        </ul>
        <ul class="d-flex justify-content-between">
            <li> <a href="#"><i class="fa-brands fa-facebook-messenger"></i></a> </li>
            <li> <a href="#"><i class="fa-brands fa-twitter"></i></a> </li>
            <li> <a href="#"><i class="fa-brands fa-vimeo-v"></i></a> </li>
            <li> <a href="#"><i class="fa-brands fa-skype"></i></a> </li>
            <li> <a href="#"><i class="fa-solid fa-wifi"></i></a> </li>
        </ul>
    </div>
</template>

<style lang="scss" scoped>
div {


    ul {
        list-style-type: none;

        li {
            padding: 10px;


            a {
                text-decoration: none;
                color: #fff;

                i {
                    padding: 10px;
                }
            }
        }
    }
}
</style>