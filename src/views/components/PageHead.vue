<template>
	<div class="border">
		<div class="zero">
			{{first}}
		</div>
		<div class="one">
			{{second}}
		</div>
	</div>
	<br>
	<div class="title">
		<h3>
			مرحبا بك في
		</h3>
		<h1>
			منصة رقم التقنية
		</h1>
	</div>
</template>
<script>
	export default {
		name: 'PageHead',
		data() {
			return {
				first: 0,
				second: 1
			}
		},
		mounted() {
			window.setInterval(() => {
				this.toggleNumbers();
			}, 3000);

		},
		methods: {
			toggleNumbers() {
				this.first = !this.first ? 1 : 0;
				this.second = !this.second ? 1 : 0;
				setTimeout(() => this.first = this.first ? 1 : 0, 100)
				setTimeout(() => this.second = this.second ? 1 : 0, 500)
			}
		}
	}
</script>
<style scoped>

	.title {
		margin-bottom: 100px;
		margin-top: 30px;
	}

	h1 {
		margin: unset;
		color: white;
		font-size: 92px;
		font-weight: 100;
	}

	h3 {
		margin: unset;
		color: white;
		font-weight: 100;
	}

	@media only screen and (max-width: 768px) {
		h1 {
			font-size: 12vw;
		}

	}

	li:before {
		content: '*';
	}

	li {
		text-align: right;
		list-style: none;
	}

	.services h2 {
		font-size: 32pt;
		font-weight: 100;
		margin-top: 0;
	}

	.border {
		border-color: white;
		border-style: solid;
		border-width: 7px;

		border-image-slice: 2;
		border-image-width: 2;
		border-image-repeat: stretch;
		border-image-source: url('data:image/svg+xml;utf8,<?xml version="1.0" encoding="UTF-8" ?><svg version="1.1" width="5" height="5" xmlns="http://www.w3.org/2000/svg"><path d="M2 1 h1 v1 h-1 z M1 2 h1 v1 h-1 z M3 2 h1 v1 h-1 z M2 3 h1 v1 h-1 z" fill="rgb(255,255,255)" /></svg>');
		border-image-outset: 2;

		display: inline-block;
		padding: 6px 8px 12px;
	}

	.zero, .one {
		margin-right: -5px;
		font-family: "Pixelar Regular W01 Regular", serif !important;
		color: white;
		font-size: 66px;
	}

	.pixel2 p {
		margin: -7px 0 0;
	}

</style>
