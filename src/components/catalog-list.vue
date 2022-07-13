<template>
	<div class="catalog-list">
		<h1>Catalog</h1>
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

<style>

</style>