<script>
export default {
    data() {
        return {
            links: [
                {
                    text: "Characters",
                    url: "#home",
                },
                {
                    text: "Movies",
                    url: "#products",
                },
                {
                    text: "Comics",
                    url: "#who",
                },
                {
                    text: "Games",
                    url: "#contacts",
                },
                {
                    text: "tv",
                    url: "#contacts",
                },
                {
                    text: "Video",
                    url: "#contacts",
                },
                {
                    text: "Fan",
                    url: "#contacts",
                },
                {
                    text: "News",
                    url: "#contacts",
                },
                {
                    text: "Shop",
                    url: "#contacts",
                },
                {
                    text: "Collectibles",
                    url: "#contacts",
                },
            ],
        }
    }
}
</script>

<template>
    <header class="container">
        <div class="row justify-content-between align-items-center p-3">
            <figure class="col-2 mb-0">
                <img src="../assets/Header-Logo/dc-logo.png" alt="Logo">
            </figure>
            <div class="col text-end">
                <a v-for="link in links" :href="link.url">{{ link.text }}</a>
            </div>
        </div>
    </header>
</template>

<style scoped>
a {
    color: #444;
    text-decoration: none;
    font-weight: bold;
    margin-left: 1rem;
}

a:hover {
    color: blue;
    border-bottom: 3px solid blue;
}
</style>
