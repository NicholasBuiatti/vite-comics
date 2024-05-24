<script>
import AppTopFooter from './AppFooterComponents/AppTopFooter.vue';
import AppMidFooter from './AppFooterComponents/AppMidFooter.vue';
import AppBottomFooter from './AppFooterComponents/AppBottomFooter.vue';
export default {
    components: {
        AppTopFooter,
        AppMidFooter,
        AppBottomFooter,
    },
    data() {
        return {

        }
    }
}
</script>

<template>

    <section id="footerImg">
        <section class="bg-primary position-relative z-1">
            <AppTopFooter />
        </section>

        <AppMidFooter />

        <section class="bg-dark position-relative z-1">
            <AppBottomFooter />
        </section>
    </section>

</template>

<style scoped>
#footerImg {
    background-image: url('../assets/footer-bg.jpg');
    background-size: cover;
}
</style>
