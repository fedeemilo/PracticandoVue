<template>
	<div>
		<hr />
		<div v-if="mostrarBoton">Usuario autenticado <ComponenteBoton /></div>
	</div>
</template>

<script>
import ComponenteBoton from './ComponenteBoton';

export default {
	name: 'ComponenteSecreto',
	data() {
		return {
			mostrarBoton: true
		};
	},
	components: {
		ComponenteBoton
	}
};
</script>

<style></style>
