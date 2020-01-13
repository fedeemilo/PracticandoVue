<template>
	<!-- Creando bucles de componentes -->
	<div>
		<h1>Creando bucles de componentes</h1>
		<button>{{ nombre }}</button>
	</div>
</template>

<script>
export default {
	name: 'ComponenteBoton',
	data() {
		return {
			nombre: 'Botón Mágico'
		};
	}
};
</script>

<style scoped>
button {
	width: 100px;
	height: 50px;
	border-radius: 25px;
	background: greenyellow;
	-webkit-appearance: none;
	font-size: 0.9rem;
	font-weight: 700;
	border: none;
}
</style>
