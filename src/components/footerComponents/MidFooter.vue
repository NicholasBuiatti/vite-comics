<script>
export default {
    data() {
        return {
            links: [
                {
                    titolo: 'DC COMICS',
                    subLinks: [
                        'Characters',
                        'Comics',
                        'Movies',
                        'TV',
                        'Games',
                        'Videos',
                        'News',
                    ]
                },
                {
                    titolo: 'SHOP',
                    subLinks: [
                        'Shop DC',
                        'Shop DC Collectibles',
                    ]
                },
                {
                    titolo: 'DC',
                    subLinks: [
                        'Terms Of Use',
                        'Privacy polic',
                        'Ad Choices',
                        'Advertising',
                        'Jobs',
                        'Subscriptions',
                        'Talent Worksh',
                        'CPSC Certific',
                        'Ratings',
                        'Shop Help',
                        'Contact Us',
                    ]
                },
                {
                    titolo: 'SITES',
                    subLinks: [
                        'DC',
                        'MAD Magazine',
                        'DC Kids',
                        'DC Universe',
                        'DC Power Visa',
                    ]
                }
            ],
        }
    }
}
</script>

<template>
    <section class="container">
        <div class="row">
            <div class="col-6 text-white p-4 d-flex flex-column flex-wrap" id="columnLinks">
                <div v-for="footLink, i in links" class="col-4 d-flex flex-column flex-wrap mb-3">
                    <h6>{{ footLink.titolo }}</h6>
                    <a v-for="subLink in footLink.subLinks" href="">{{ subLink }}</a>
                </div>

            </div>
            <figure class="col-6 text-end mb-0 position-relative">
                <img src="../../assets/Footer-Bottom-Img/dc-logo-bg.png" alt="">
            </figure>
        </div>

    </section>
</template>

<style scoped>
#columnLinks {
    height: 25rem;
}

figure {
    height: 25rem;
}

img {
    height: 30rem;
    position: absolute;
    transform: translate(-100%, -10%);
}
</style>