<template>
	<div id="app">
		<div class="container">
			<div class="row">
				<Navegacion />
			</div>
			<div class="row">
				<h1>Mi web</h1>
				<p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Maiores, numquam ipsam maxime atque impedit eos ex? Obcaecati temporibus, ducimus sint praesentium exercitationem eum aspernatur saepe eveniet rem animi quidem delectus!
				Libero itaque aspernatur facilis provident asperiores maxime! Sapiente, tenetur odit error alias repellendus accusamus deserunt recusandae libero ullam non numquam est illum sunt modi doloremque laborum reprehenderit cumque adipisci fuga?
				Eveniet eligendi iure voluptas suscipit, totam aut aspernatur laboriosam laborum magnam? Quia repudiandae iste fugiat libero quo natus illo. Voluptatum similique repellat maiores esse dignissimos libero qui rem itaque ipsam.</p>
			</div>
		</div>
	</div>
</template>

<script>
	import Navegacion from './components/Navegacion.vue';

export default {
	name: 'app',
	components: {
		Navegacion
	}
};
</script>

<style>
#app {
	font-family: 'Avenir', Helvetica, Arial, sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	text-align: center;
	color: #2c3e50;
	margin-top: 60px;
}
</style>
