<template>
	<div class="catalog-list">
		<catalog-item />
		<catalog-item />
		<catalog-item />
		<catalog-item />
		<catalog-item />
		<catalog-item />
	</div>
</template>

<script>
	import catalogItem from './catalog-item.vue'

	export default {
		name: "catalog-list",
		components: {
			catalogItem
		},
		props: {},
		data() {
			return {
				
			}
		},
		computed: {},
	}
</script>

<style lang="scss">
	.catalog-list {
		display: grid;
		grid-template-columns: 1fr 1fr 1fr;
		grid-template-rows: repeat(2, auto);
		column-gap: 17px;
		row-gap: 16px;
		list-style-type: none;
		padding: 0;
		margin: 0;
	}
	@media screen and (max-width: 1179px) {
		.catalog-list {
			grid-template-columns: 1fr 1fr;
		}
	}
	@media screen and (max-width: 767px) {
		.catalog-list {
			grid-template-columns: 1fr;
		}
	}
</style>