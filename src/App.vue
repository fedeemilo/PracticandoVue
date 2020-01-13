<template>
	<div id="app">
		<MiComponente v-for="x in 2" v-bind:key="x" />

		<ComponenteBoton v-for="y in 5" v-bind:key="y" />

		<ComponenteSecreto />
	</div>
</template>

<script>
import MiComponente from './components/MiComponente.vue';
import ComponenteBoton from './components/ComponenteBoton.vue';
import ComponenteSecreto from './components/ComponenteSecreto.vue';

export default {
	name: 'app',
	components: {
		MiComponente,
		ComponenteBoton,
		ComponenteSecreto
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
