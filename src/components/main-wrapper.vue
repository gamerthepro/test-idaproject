<template>
	<div class="main-wrapper">
		<valid-form />
		<catalog-list />
	</div>
</template>

<script>
	import catalogList from './catalog-list.vue'
	import validForm from './valid-form.vue'

	export default {
		name: "main-wrapper",
		components: {
			catalogList,
			validForm
		},
		props: {},
		data() {},
		computed: {},
		methods: {},
		watch: {},
		mounted() {}
	}
</script>

<style lang="scss">
	.main-wrapper {
		display: flex;
		flex-direction: row;
		justify-content: center;
		align-items: center;
		max-width: 1440px;
		margin: 0 auto;
		background: rgba(255, 254, 251, 0.8);
	}
</style>