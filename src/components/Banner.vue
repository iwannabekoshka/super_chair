<template>
	<section class="banner">
		<div class="wrapper">
			<h1 class="title">Супер кошки</h1>
			<p>Koshki is love, koshki is life. Lorem ipsum dolor sit amet koshka.</p>
			<a href="" class="button">Подробнее</a>
		</div>
	</section>
</template>

<script>

	export default {
		name: "Banner",
	}
</script>

<style scoped>
	.banner {
		background: linear-gradient( rgba(0, 0, 0, 0.3), rgba(0, 0, 0, 0.3) ), url("../assets/img/banner.jpg");
		background-repeat: no-repeat;
		background-size: cover;
		background-position: center center;
		padding: 150px 0px;

		color: white;

		margin-bottom: 80px;
	}
	.title {
		font-size: 48px;
		margin-bottom: 50px;
		font-weight: bold;
	}
	p {
		margin-bottom: 64px;
		width: 320px;
		line-height: 20px;
	}
	.button {
		border-color: white;
	}
	.button:hover {
		background-color: white;
		color: var(--color-dark);
	}
</style>