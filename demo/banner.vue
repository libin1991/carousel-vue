<template>
    <div class="banner-wrap">
        <carousel :indicators="true" :auto="3000" :responsive="36.533333333333334" :on-slid-end="onSlidEnd">
            <div v-for="(item, index) in banner" :key="index"></div>
        </carousel>
    </div>
</template>
<script>
    import Carousel from '../Carousel';
    export default {
        components: {
            Carousel
        },
        methods: {
            onSlidEnd() {
                // TODO: 轮播切换完成时的回调
            }
        }
    }
</script>
