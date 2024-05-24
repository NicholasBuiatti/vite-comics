<script>
export default {
    data() {
        return {
            socialMedia: [
                {
                    social: 'Facebook',
                    logo: 'footer-facebook.png',
                },
                {
                    social: 'Youtube',
                    logo: 'footer-youtube.png',
                },
                {
                    social: 'Periscope',
                    logo: 'footer-periscope.png',
                },
                {
                    social: 'Twitter',
                    logo: 'footer-twitter.png',
                },
                {
                    social: 'Pinterest',
                    logo: 'footer-pinterest.png',
                },
            ]
        }
    },
    methods: {
        getImg(imgFootTop) {
            let risultato = new URL(`../../assets/Footer-Bottom-Img/${imgFootTop}`, import.meta.url);
            return risultato.href;
        },
    },
}
</script>

<template>
    <section class="position-relative z-1 container p-4">
        <div class="row justify-content-between align-items-center">
            <button type="button" class="col-2 btn text-white border border-4 border-primary rounded-0 btn-lg">SIGN-UP
                NOW</button>
            <h6 class="text-primary col text-end">FOLLOW US</h6>
            <div class="col-3 text-end">
                <img v-for="social in socialMedia" :src="getImg(social.logo)" alt="">
            </div>
        </div>

    </section>
</template>

<style scoped>
img {
    margin-left: 1rem;
}
</style>