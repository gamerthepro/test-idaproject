<template>
	<div class="main-wrapper"></div>
</template>

<script>
	export default {
		name: "main-wrapper",
		components: {},
		props: {},
		data() {
			return {
				title: "main"
			}
		},
		computed: {},
		methods: {},
		watch: {},
		mounted() {
			console.log('hello Artem')
		}
	}
</script>

<style>
	.main {
		display: flex;
		justify-content: center;
		align-items: center;
		max-width: 1440px;
		margin: 0 auto;
	}
</style>