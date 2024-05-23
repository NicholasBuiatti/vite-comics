<script>
export default {
    data() {
        return {
            links: [
                {
                    text: 'Digital Comics',
                    img: "../../assets/Footer-Top-Img/buy-comics-digital-comics.png",
                    url: "#home",
                },
                {
                    text: 'DC Merchandise',
                    img: "../../assets/Footer-Top-Img/buy-comics-merchandise.png",
                    url: "#products",
                },
                {
                    text: 'Subscription',
                    img: "../../assets/Footer-Top-Img/buy-comics-subscriptions.png",
                    url: "#who",
                },
                {
                    text: 'Comic Shop Locator',
                    img: "../../assets/Footer-Top-Img/buy-comics-shop-locator.png",
                    url: "#contacts",
                },
                {
                    text: 'DC Power Visa',
                    img: "../../assets/Footer-Top-Img/buy-dc-power-visa.svg",
                    url: "#contacts",
                },
            ],

        }
    }
}
</script>

<template>
    <div class="row">
        <div v-for="link in links" class="col row align-items-center">
            <figure class="w-25 mb-0">
                <img class="col-12" src="../../assets/Footer-Top-Img/buy-comics-digital-comics.png" alt="">
            </figure>
            <a href="" class="col">{{ link.text }}</a>
        </div>
    </div>
</template>

<style scoped>
a {
    color: white;
    text-decoration: none;
}
</style>