<template>
	<div class="valid-form">
		<h1 class="valid-form__title">Добавление товара</h1>
		<form class="form">
			<P class="form__name form__name-mark-on">Наименование товара</P>
			<input class="form__input form__input-error" 
			type="name"
			placeholder="Введите наименование товара"
			>
			<span className="form__error" id="">поле являеться обязятальным</span>
			<P class="form__name">Описание товара</P>
			<textarea class="form__input form__input-text"
			type="text"
			placeholder="Введите описание товара"
			></textarea>
			<P class="form__name form__name-mark-on">Ссылка на изображение товара</P>
			<input class="form__input" 
			type="url-image"
			placeholder="Введите ссылку"
			>
			<span className="form__error" id=""></span>
			<P class="form__name form__name-mark-on">Цена товара</P>
			<input class="form__input" 
			type="text"
			placeholder="Введите цену"
			>
			<span className="form__error" id=""></span>
			<button class="form__button">Добавить товар</button>
		</form>
	</div>
</template>

<script>
	export default {
		name: "valid-form",
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
	.valid-form {
		display: flex;
		flex-direction: column;

		.valid-form__title {
			font-family: 'Source Sans Pro';
			font-style: normal;
			font-weight: 600;
			font-size: 28px;
			line-height: 35px;
			text-align: start;
			margin: 0 0 16px 0;
			color: #3F3F3F;
		}
		.form {
			display: flex;
			flex-direction: column;
			align-items: flex-start;
			padding: 24px;
			box-shadow: 0px 20px 30px rgba(0, 0, 0, 0.04), 0px 6px 10px rgba(0, 0, 0, 0.02);
			border-radius: 4px;
			background-color: rgba(255, 254, 251, 0.8);
			.form__name {
				display: flex;
				position: relative;
				font-family: 'Source Sans Pro';
				font-style: normal;
				font-weight: 400;
				font-size: 10px;
				line-height: 13px;
				letter-spacing: -0.02em;
				color: #49485E;
				margin: 0;
			}
			.form__name-mark-on::before {
				content: "";
				position: absolute;
				right: -4px;
				top: 0px;
				width: 4px;
				height: 4px;
				background: #FF8484;
				border-radius: 4px;
			}
			.form__input {
				display: flex;
				position: relative;
				min-height: 36px;
				width: 100%;
				margin: 4px 0 0;
				padding: 0;
				background: #FFFEFB;
				border: none;
				box-shadow: 0px 2px 5px rgba(0, 0, 0, 0.1);
				border-radius: 4px;
				cursor: pointer;
			}
			.form__input::placeholder {
				display: flex;
				padding: 10px 0 0 16px;
				font-family: 'Source Sans Pro';
				font-style: normal;
				font-weight: 400;
				font-size: 12px;
				line-height: 15px;
				text-align: left;
				color: #B4B4B4;
			}
			.form__input-error {
				border: 1px solid #FF8484;
				box-shadow: 0px 2px 5px rgba(0, 0, 0, 0.1);
				border-radius: 4px;
			}
			.form__error {
				font-family: 'Source Sans Pro';
				font-style: normal;
				font-weight: 400;
				font-size: 8px;
				line-height: 10px;
				letter-spacing: -0.02em;
				color: #FF8484;
				margin: 4px 0 2px;
				min-height: 10px;
			}
			.form__input-text {
				min-height: 108px;
				resize: none;
			}
			.form__button {
				width: 284px;
				height: 36px;
				color: #B4B4B4;
				background: #EEEEEE;
				margin-top: 8px;
				border-radius: 10px;
				font-family: 'Inter';
				font-style: normal;
				font-weight: 600;
				font-size: 12px;
				line-height: 15px;
				text-align: center;
				letter-spacing: -0.02em;
				border: none;
				cursor: pointer;
			}
			.form__button:hover {
			background: #e6e6e4;
			}
		}
	}
</style>