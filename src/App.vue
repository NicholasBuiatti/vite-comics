<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';

export default {
	components: {
		AppHeader,
		AppMain,
		AppFooter,
	},
	data() {
		return {

		}
	}
}
</script>

<template>
	<AppHeader />

	<AppMain />

	<AppFooter />

</template>

<style scoped></style>

<!-- getImg(path) {
	let risultato = new URL(`../assets/img/${path}`, import.meta.url);
	return risultato.href;
}, -->
