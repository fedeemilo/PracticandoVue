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
		<!-- La etiqueta es div vacía es poblada por los valores de mensajes.texto3
		gracias al atributo de vue llamado v-html -->
		<!-- *No es buena idea añadir éste atributo al nodo central en que estamos
		desplegando nuestra app* -->
		<div v-html="mensajes.texto3"></div>
		<hr />

		<!-- Bucles y condicionales con Vue.js -->
		<h1>Bucles y condicionales</h1>
		<!-- Despliegue básico de un arreglo -->
		<div>
			<!-- *Forma básica, pero no la deseada* -->
			{{ colores[0] }}
			{{ colores[1] }}
			{{ colores[2] }}
			{{ colores[3] }}
		</div>
		<!-- Desplegar listas -->
		<div>
			<h2>Desplegar Listas</h2>
			<ul>
				<li v-bind:key="color" v-for="color in colores">{{ color }}</li>
			</ul>
		</div>
		<!-- Desplegar listas de objetos -->
		<div>
			<h2>Desplegar listas de objetos</h2>
			<div v-bind:key="colorObj" v-for="colorObj in coloresObjetos">
				Español: {{ colorObj.nombre }} <br />
				Inglés: {{ colorObj.nombreIngles }}
				<p>--------------------------------------------</p>
			</div>
		</div>
		<!-- Utilizando Bootstrap dentro de Vue -->
		<h1>Bootstrap 4 en Vue</h1>
		<ul class="nav">
			<li class="nav-item">
				<a class="nav-link active" href="#">Active</a>
			</li>
			<li class="nav-item">
				<a class="nav-link" href="#">Link</a>
			</li>
			<li class="nav-item">
				<a class="nav-link" href="#">Link</a>
			</li>
			<li class="nav-item">
				<a class="nav-link disabled" href="#" tabindex="-1" aria-disabled="true"
					>Disabled</a
				>
			</li>
		</ul>
		<div></div>
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
			},
			colores: ['azul', 'verde', 'amarillo', 'rojo'],
			coloresObjetos: [
				{ nombre: 'rojo', nombreIngles: 'red' },
				{ nombre: 'azul', nombreIngles: 'blue' },
				{ nombre: 'amarillo', nombreIngles: 'yellow' },
				{ nombre: 'verde', nombreIngles: 'green' }
			]
		};
	}
};
</script>

<style scoped>
li {
	list-style: none;
	margin-left: -3rem;
}
</style>
