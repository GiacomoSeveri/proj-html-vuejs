<script>
export default {
    name: 'InfoFooter',
    data() {
        return {
            items: [
                { icon: '01 (4)', info: 'Phone Number: +80012 345 678 912' },
                { icon: '02', info: 'Email: youremail@gmail.com' },
                { icon: '03', info: 'Address: 30 North West New York 240' }
            ]
        }
    }
}
</script>

<template>
    <div class="d-flex justify-content-center">
        <div class="mx-3 ">
            <a href="#"><img src="imgs/01 (4).png" alt="" class="mx-2"></a>
            <span>Phone Number: +80012 345 678 912</span>
        </div>
        <div class="mx-3 ">
            <a href="#"><img src="imgs/02.png" alt="" class="mx-2"></a>
            <span>Email: youremail@gmail.com</span>
        </div>
        <div class="mx-3 ">
            <a href="#"><img src="imgs/03.png" alt="" class="mx-2"></a>
            <span>Address: 30 North West New York 240</span>
        </div>
    </div>
</template>

<style lang="scss" scoped>

</style>