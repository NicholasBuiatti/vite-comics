<script>
export default {
    data() {
        return {
            links: [
                {
                    text: 'Digital Comics',
                    img: "buy-comics-digital-comics.png",
                    url: "#home",
                },
                {
                    text: 'DC Merchandise',
                    img: "buy-comics-merchandise.png",
                    url: "#products",
                },
                {
                    text: 'Subscription',
                    img: "buy-comics-subscriptions.png",
                    url: "#who",
                },
                {
                    text: 'Comic Shop Locator',
                    img: "buy-comics-shop-locator.png",
                    url: "#contacts",
                },
                {
                    text: 'DC Power Visa',
                    img: "buy-dc-power-visa.svg",
                    url: "#contacts",
                },
            ],

        }
    },
    methods: {
        getImg(imgFootTop) {
            let risultato = new URL(`../../assets/Footer-Top-Img/${imgFootTop}`, import.meta.url);
            return risultato.href;
        },
    }
}
</script>

<template>
    <section class="container p-5">
        <div class="row">
            <div v-for="link in links" class="col row align-items-center">
                <figure class="mb-0">
                    <img class="col-12" :src="getImg(link.img)" alt="">
                </figure>
                <a href="" class="col">{{ link.text }}</a>
            </div>
        </div>
    </section>
</template>

<style scoped>
a {
    color: white;
    text-decoration: none;
}

figure {
    width: 5rem;
}
</style>