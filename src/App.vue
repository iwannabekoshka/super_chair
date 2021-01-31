<template>
	<div id="app">
		<Header />
		<Banner />
		<Goods />
	</div>
</template>

<script>
	import Header from "@/components/Header";
	import Banner from "@/components/Banner";
	import Goods from "@/components/Goods";
	export default {
		name: 'App',
		components: {Goods, Banner, Header}
	}
</script>

<style>
	@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700&display=swap');
	* {
		margin: 0;

		--color-light: #EFEFEF;
		--color-accent: #66C05D;
		--color-dark: #333333;
	}
	body {
		background-color: var(--color-light);

		font-family: 'Roboto', sans-serif;
		font-size: 14px;
		color: var(--color-dark)
	}
	a {
		color: inherit;
		text-decoration: none;
	}
	hr {
		border: 1px solid var(--color-light)
	}
	.wrapper {
		max-width: 1110px;
		margin: 0 auto;
		padding: 0 1rem;
	}
	.button {
		padding: 13px 27px;
		background-color: transparent;
		border: 2px solid var(--color-accent);
		border-radius: 1000px;
		cursor: pointer;
		transition: .3s ease;
	}
	.button:hover {
		background-color: var(--color-accent);
		color: white;
	}
</style>
