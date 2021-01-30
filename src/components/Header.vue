<template>
	<header>
		<nav class="nav">
			<div class="wrapper">
				<ul>
					<li><a href="#">Доставка</a></li>
					<li><a href="#">Оплата</a></li>
					<li><a href="#">Отзывы</a></li>
					<li><a href="#">Вопрос-ответ</a></li>
					<li><a href="#">Контакты</a></li>
				</ul>
			</div>
		</nav>

		<div class="bg-white">
			<div class="wrapper">
				<div class="header">
					<div class="logo">
						<img :src="cat" alt="logo">
						BEAUTY
					</div>

					<div class="back-call">
						<span class="phone">8-999-888-77-66</span>
						<button class="button">Обратный звонок</button>
					</div>
				</div>
			</div>
			<hr>
			<nav class="main-menu">
				<div class="wrapper">
					<ul>
						<li><a href="#">Парикмахерская</a></li>
						<li><a href="#">Барбершоп</a></li>
						<li><a href="#">Маникюр</a></li>
						<li><a href="#">Педикюр</a></li>
						<li><a href="#">Массаж</a></li>
						<li><a href="#">Мебель</a></li>
					</ul>
				</div>
			</nav>
		</div>
	</header>
</template>

<script>
	import logo from '../assets/img/logo.svg'
	import cat from '../assets/img/cat.svg'
	export default {
		name: "Header",
		data() {
			return {
				logo,
				cat
			}
		}
	}
</script>

<style scoped>
	header {

	}
	.nav {
		padding: 1.1rem 0px;
	}
	ul {
		display: flex;
		justify-content: center;

		list-style-type: none;
		padding: 0;
	}
	li {
		margin: 0 1rem;
	}
	hr {
		margin: 1.1rem -0px;
	}
	.bg-white {
		background-color: #fff;
		padding: 1.4rem 0;
	}
	.header {
		display: flex;
		align-items: center;
		justify-content: space-between;
	}
	.logo {
		display: flex;
		align-items: center;

		color: var(--color-accent);
		font-weight: bold;
		font-size: 2.6rem;
		letter-spacing: 0.1em;
	}
	.logo > img {
		width: 80px;
	}

	.phone {
		font-size: 1.14rem;
		margin-right: 2.9rem;
	}

	.main-menu {
		font-size: 1rem;
		color: black;
	}
</style>