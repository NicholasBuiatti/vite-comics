<script>
import TopFooter from './footerComponents/TopFooter.vue';
import MidFooter from './footerComponents/MidFooter.vue';
import BottomFooter from './footerComponents/BottomFooter.vue';
export default {
    components: {
        TopFooter,
        MidFooter,
        BottomFooter,
    },
    data() {
        return {

        }
    }
}
</script>

<template>

    <section id="footerImg">
        <section class="bg-primary">
            <TopFooter />
        </section>

        <MidFooter />

        <section class="bg-dark">
            <BottomFooter />
        </section>
    </section>

</template>

<style scoped>
#footerImg {
    background-image: url('../assets/footer-bg.jpg');
    background-size: cover;
    position: relative;
}
</style>
