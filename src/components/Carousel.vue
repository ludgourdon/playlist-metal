<template>
    <carousel :data="data"></carousel>
</template>

<script>
    import VueCarousel from '@chenfengyuan/vue-carousel';

    export default {
        data() {
            return {
                data: [
                    '<div class="example-slide">Slide 1</div>',
                    '<div class="example-slide">Slide 2</div>',
                    '<div class="example-slide">Slide 3</div>',
                ],
            };
        },
    };
</script>

<style scoped>
    .example-slide {
        align-items: center;
        background-color: #666;
        color: #999;
        display: flex;
        font-size: 1.5rem;
        justify-content: center;
        min-height: 10rem;
        height:100vh;
    }
</style>