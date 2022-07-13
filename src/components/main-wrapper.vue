<template>
	<div class="main-wrapper"></div>
	<p>{{title}}</p>
</template>

<script>
	export default {
		name: "main-wrapper",
		components: {},
		props: {},
		data() {
			return {
				title: "hello Artem"
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
	.main-wrapper {
		display: flex;
		justify-content: center;
		align-items: center;
		max-width: 1440px;
		margin: 0 auto;
	}
</style>