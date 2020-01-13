<template>
	<div>
		<hr />
		<div v-if="mostrarBoton == 'clave'">Usuario autenticado <ComponenteBoton /></div>
        <div v-else-if="mostrarBoton == ''">No ingresaste ningun valor</div>
        <div v-else>Error</div>
        <!-- ***show oculta la informacion, en cambio v-if la quita del document*** -->
        <!-- Es màs recomendable el uso de v-if para liberar memoria y optimizar la app -->
        <div v-show="mostrarBoton == 'clave'"><ComponenteBoton /></div>
	</div>
</template>

<script>
import ComponenteBoton from './ComponenteBoton';

export default {
	name: 'ComponenteSecreto',
	data() {
		return {
			mostrarBoton: 'clave'
		};
	},
	components: {
		ComponenteBoton
	}
};
</script>

<style></style>
