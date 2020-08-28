<template>
	<div id="app">
		<HelloWorld />
	</div>
</template>

<script>
	import HelloWorld from './components/HelloWorld.vue'

	export default {
		name: 'App',
		components: {
			HelloWorld
		}
	}
</script>

<style>
	@import "~pixel-borders/docs/styles/pixel-borders.css";

	@font-face {
		font-family: Raqami;
		src: url("./assets/fonts/Raqami v2.0.otf") format("opentype");
	}

	@font-face {
		font-family: "Pixelar Regular W01 Regular";
		src: url("./assets/fonts/b2e75c336df191233b3096682c9ee6be.eot"); /* IE9*/
		src: url("./assets/fonts/b2e75c336df191233b3096682c9ee6be.eot?#iefix") format("embedded-opentype"), /* IE6-IE8 */ url("./assets/fonts/b2e75c336df191233b3096682c9ee6be.woff2") format("woff2"), /* chrome、firefox */ url("./assets/fonts/b2e75c336df191233b3096682c9ee6be.woff") format("woff"), /* chrome、firefox */ url("./assets/fonts/b2e75c336df191233b3096682c9ee6be.ttf") format("truetype"), /* chrome、firefox、opera、Safari, Android, iOS 4.2+*/ url("./assets/fonts/b2e75c336df191233b3096682c9ee6be.svg#Pixelar Regular W01 Regular") format("svg"); /* iOS 4.1- */
	}

	#app {
		height: 100%;
		width: 100%;
		font-family: Raqami, Helvetica, Arial, sans-serif;
		-webkit-font-smoothing: antialiased;
		-moz-osx-font-smoothing: grayscale;
		text-align: center;
		color: #2c3e50;
	}

	html, body {
		height: 100%;
		width: 100%;
		padding: 0;
		margin: 0;
	}

	* {
		box-sizing: border-box;
		direction: rtl;
	}
</style>
