<template>

	<div class="catalog-list">
		<button class="list__button">По умолчанию <img src="../image/ListButtonImage.svg" alt="галочка"></button>
		<div class="list__container">
			<catalog-item />
			<catalog-item />
			<catalog-item />
			<catalog-item />
			<catalog-item />
			<catalog-item />
		</div>
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
		display: block;
		position: relative;
		.list__button {
			display: block;
			position: absolute;
			width: 122px;
			height: 36px;
			right: 0px;
			background: #FFFEFB;
			box-shadow: 0px 2px 5px rgba(0, 0, 0, 0.1);
			border-radius: 4px;
			border: none;
			font-family: 'Source Sans Pro';
			font-style: normal;
			font-weight: 400;
			font-size: 12px;
			line-height: 15px;
			font-family: 'Source Sans Pro';
			color: #B4B4B4;
		}
		.list__button:hover {
			background: #EEEEEE;
		}
		.list__container {
			display: grid;
			grid-template-columns: 1fr 1fr 1fr;
			grid-template-rows: repeat(2, auto);
			column-gap: 17px;
			row-gap: 16px;
			list-style-type: none;
			padding: 0;
			margin: 51px auto 0;
		}
			@media screen and (max-width: 1439px) {
		.list__container {
			grid-template-columns: 1fr 1fr;
		}
		}
		@media screen and (max-width: 1179px) {
			.list__container {
				grid-template-columns: 1fr;
			}
		}
	}
</style>