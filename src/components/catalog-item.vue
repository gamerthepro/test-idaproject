<template>
	<div class="catalog-item">
		<img class="item__image" src="../image/image.svg" alt="картинка товара"/>
		<h1 class="item__name">Наименование товара</h1>
		<p class="item__description">Довольно-таки интересное описание товара в несколько строк. Довольно-таки интересное описание товара в несколько строк</p>
		<p class="item__price">10 000 руб.</p>
	</div>
</template>

<script>
	export default {
		name: "catalog-item",
		components: {},
		props: {},
		data() {
			return {
				
			}
		},
		computed: {},
	}
</script>

<style lang="scss">
	.catalog-item {
		display: flex;
		flex-direction: column;
		align-items: flex-start;
		max-width: 332px;
		min-height: 423px;
		background: #FFFEFB;
		box-shadow: 0px 20px 30px rgba(0, 0, 0, 0.04), 0px 6px 10px rgba(0, 0, 0, 0.02);
		border-radius: 4px;
		.item__image {
			width: 332px;
			height: 200px;
		}
		.item__name {
			font-family: 'Source Sans Pro';
			font-style: normal;
			font-weight: 600;
			font-size: 20px;
			line-height: 25px;
			color: #3F3F3F;
			margin: 16px;
		}
		.item__description {
			text-align: left;
			font-family: 'Source Sans Pro';
			font-style: normal;
			font-weight: 400;
			font-size: 16px;
			line-height: 20px;
			color: #3F3F3F;
			margin: 0 16px 16px 16px;
		}
		.item__price {
			font-family: 'Source Sans Pro';
			font-style: normal;
			font-weight: 600;
			font-size: 24px;
			line-height: 30px;
			color: #3F3F3F;
			margin: 16px 16px 24px 16px;
		}
	}
</style>