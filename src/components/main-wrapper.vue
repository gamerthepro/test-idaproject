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
		align-items: flex-start;
		justify-content: center;
		max-width: 1440px;
		padding: 32px;
		margin: 0;
		background: rgba(255, 254, 251, 0.8);
	}
</style>