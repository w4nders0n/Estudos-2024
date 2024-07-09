<template>
	<div>
		<h1>Olá vue</h1>
		<multiplosEventos />
	</div>
</template>
<script>
	import multiplosEventos from './multiplosEventos.vue'
	export default{
		nome:"primeiroComponente",
		components: {
			multiplosEventos
		}
	}
</script>