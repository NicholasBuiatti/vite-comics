<script>
import Header from './components/Header.vue';
import Main from './components/Main.vue';
import Footer from './components/Footer.vue';

export default {
	components: {
		Header,
		Main,
		Footer,
	},
	data() {
		return {

		}
	}
}
</script>

<template>
	<Header />

	<Main />

	<Footer />

</template>

<style scoped></style>

<!-- getImg(path) {
	let risultato = new URL(`../assets/img/${path}`, import.meta.url);
	return risultato.href;
}, -->
