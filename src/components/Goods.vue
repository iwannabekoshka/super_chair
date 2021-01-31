<template>
	<section>
		<div class="wrapper">
			<div class="grid">
				<div class="title">
					<h3>Специальные предложения</h3>
				</div>
				<div class="shipping">
					<img src="../assets/img/car.svg" alt="Shipping">
				</div>
				<div class="card">
					<img class="good" src="../assets/img/goods_1.jpg" alt="">
					<p class="good-title">кошка-панкреотит</p>
					<p class="price">Бесценно</p>
					<a class="button">Купить</a>
				</div>
				<div class="card">
					<img class="good" src="../assets/img/goods_1.jpg" alt="">
					<p class="good-title">кошка-панкреотит</p>
					<p class="price">Бесценно</p>
					<a class="button">Купить</a>
				</div>
				<div class="card">
					<img class="good" src="../assets/img/goods_1.jpg" alt="">
					<p class="good-title">кошка-панкреотит</p>
					<p class="price">Бесценно</p>
					<a class="button">Купить</a>
				</div>
				<div class="card">
					<img class="good" src="../assets/img/goods_1.jpg" alt="">
					<p class="good-title">кошка-панкреотит</p>
					<p class="price">Бесценно</p>
					<a class="button">Купить</a>
				</div>
				<div class="get-email">
					<h3>Получайте котов в руки и в сердце</h3>
					<p>Каждый день мы разыгрываем котов!</p>
					<input type="email">
				</div>
				<div class="map">
					<h3>Заходите к нам</h3>
					<p>У нас нет магазинов, но вы заходите!</p>
					<div class="button">Я карта</div>
				</div>
			</div>
		</div>
	</section>
</template>

<script>
	export default {
		name: "Goods"
	}
</script>

<style scoped>
	.good {
		width: 155px;
	}
	.shipping {
		text-align: center;
	}
	.grid {
		display: grid;
		grid-template-columns: repeat(4, 1fr);
		grid-gap: 0 30px;
	}
	.title {
		display: flex;
		align-items: center;

		font-size: 24px;
		font-weight: bold;

		grid-column: 1/4;
		grid-row: 1/2;
	}
	.shipping {
		grid-column: 4/5;
		grid-row: 1/2;
	}
	.get-email {
		grid-column: 1/3;
		grid-row: 3/4;
	}
	.map {
		grid-column: 3/5;
		grid-row: 3/4;
	}

	.card {
		background-color: #fff;
		text-align: center;
		padding: 15px 30px;
	}
	.good, .good-title {
		margin-bottom: 30px;
	}
	.price {
		font-size: 21px;
		font-weight: 500;
		color: black;

		margin-bottom: 40px;
	}

	.get-email, .map {
		background-color: var(--color-accent);
	}

	.button {
		padding: 9px 40px;
		background-color: var(--color-accent);
		color: white;

		transition: .3s ease;
	}
	.button:hover {
		background-color: transparent;
		color: var(--color-dark);
	}
</style>