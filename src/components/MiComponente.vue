<template>
	<div class="MiComponente">
		<h1>Ésta es mi primera app contruida con Vue.js</h1>
		<h3>
			Tiene una curva de aprendizaje muy baja y he aprendido mucho en sólo 2
			días!
		</h3>
		<h2>Autor: {{ libro.autor }}</h2>
		<h3>Libro: {{ libro.titulo }}</h3>
		<hr />

		<!-- Concatenación y operaciones básicas -->
		<!-- *Ésto es un ejemplo. No es lo recomendado* -->
		<h1>{{ mensajes.texto1 + mensajes.texto2 }}</h1>
		<hr />

		<!-- Mostrar texto en formato html -->
		
	</div>
</template>

<script>
// Con éste comando exporto el componente dentro de la app
export default {
	// Defino las propiedades del componente
	name: 'MiComponente',
	data() {
		return {
			libro: {
				autor: 'Federico Milone',
				titulo: 'Aprendiendo Vue'
			},
			mensajes: {
				texto1: 'Vue',
				texto2: '.js',
				texto3: '<h1>Lorem ipsum </h1> <i>dolor sit amet</i>'
			}
		};
	}
};
</script>

<style scoped></style>
