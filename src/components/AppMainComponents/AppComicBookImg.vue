<script>
export default {
    props: ["singleComicBook"]
}
</script>

<template>
    <div>
        <figure>
            <img :src="singleComicBook.thumb" alt="" class="col-12 h-100">
        </figure>
        <p class="text-white">{{ singleComicBook.series.toUpperCase() }}</p>

    </div>
</template>

<style scoped>
#changeImg {
    transform: translateY(-50%);
}
</style>