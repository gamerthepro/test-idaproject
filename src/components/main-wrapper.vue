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
		justify-content: space-around;
		align-items: flex-start;
		padding: 32px;
		margin: 0 auto;
		background: rgba(255, 254, 251, 0.8);
	}
	@media screen and (max-width: 767px) {
			.main-wrapper {
				flex-direction: column;
				align-items: center;
			}
		}
</style>