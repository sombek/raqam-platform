<template>
	<div class="HomePage">
		<div class="container">
			<PageHead/>

			<Services/>

			<Buttons/>

			<AppFooter/>
		</div>
	</div>
</template>

<script>
	import PageHead from "./components/PageHead";
	import Services from "./components/Services";
	import Buttons from "./components/Buttons";
	import AppFooter from "./components/AppFooter";

	export default {
		name: 'HomePage',
		components: {AppFooter, Buttons, Services, PageHead},
	}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
	.container {
		height: 100%;
		position: relative;
	}

	.HomePage {
		height: 100%;
		width: 100%;
		background-color: #ff6532;
		padding-top: 60px;
		display: inline-table;
	}
</style>
