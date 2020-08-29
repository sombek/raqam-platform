<template>
	<div class="buttons">
		<div class="pixelButton"
			 onclick="window.open('https://wa.me/966595585131/?text=%D9%85%D8%B1%D8%AD%D8%A8%D9%8B%D8%A7%D8%8C+%D8%A7%D8%B1%D9%8A%D8%AF+%D8%A7%D9%84%D8%A5%D8%B3%D8%AA%D9%81%D8%B3%D8%A7%D8%B1+%D8%B9%D9%86+%D8%AE%D8%AF%D9%85%D8%A7%D8%AA+%D9%85%D9%86%D8%B5%D8%A9+%D8%B1%D9%82%D9%85+%D8%A7%D9%84%D8%AA%D9%82%D9%86%D9%8A%D8%A9')">
			<p>
				الإستعلام عن خدماتنا
			</p>
		</div>
		<div class="pixelButton" onclick="window.location.href = 'tel:0595585131'">
			<p>
				الإتصال بنا
			</p>
		</div>
	</div>
</template>
<script>
	export default {
		name: 'Buttons'
	}
</script>
<style scoped>

	@media only screen and (max-width: 768px) {
		h1 {
			font-size: 12vw;
		}

		div.pixelButton {
			margin: 10px;
		}

	}

	.buttons {
		height: 200px;
	}

	.pixelButton {
		padding: 10px 10px;
		position: relative;
		background: white;

		z-index: 2;
		margin: auto 20px;
		font-size: 25px;
		color: #ff6532;

		display: inline-block;
		vertical-align: top;

		width: 250px;
		height: auto;

		cursor: pointer;

		-webkit-touch-callout: none;
		-webkit-user-select: none;
		-khtml-user-select: none;
		-moz-user-select: none;
		-ms-user-select: none;
		user-select: none;
	}

	.pixelButton:active {
		top: 2px;
	}

	.pixelButton::before {
		content: "";
		display: block;
		position: absolute;
		top: 10px;
		bottom: 10px;
		left: -10px;
		right: -10px;
		background: white;
		z-index: -1;
	}

	.pixelButton::after {
		content: "";
		display: block;
		position: absolute;
		top: 4px;
		bottom: 4px;
		left: -6px;
		right: -6px;
		background: white;
		z-index: -1;
	}

	.pixelButton p {
		margin: -7px 0 0;
	}

</style>
