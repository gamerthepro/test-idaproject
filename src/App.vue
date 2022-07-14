<template>
	<div id="app">
		<main-wrapper />
	</div>
</template>

<script>
	import MainWrapper from './components/main-wrapper.vue'

export default {
	name: 'app',
	components: {
		MainWrapper
	}
}
</script>

<style>
#app {
	font-family: Avenir, Helvetica, Arial, sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	max-width: 1440px;
	margin: 0 auto;
	text-align: center;
}
</style>
