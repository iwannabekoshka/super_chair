<template>
	<div id="app">
		<Header />
	</div>
</template>

<script>
	import Header from "@/components/Header";
	export default {
		name: 'App',
		components: {Header}
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
		padding: .7rem 1.8rem;
		background-color: transparent;
		border: 2px solid var(--color-accent);
		border-radius: 1000px;
	}
</style>
