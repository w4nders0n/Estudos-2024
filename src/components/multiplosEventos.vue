<template>
	<div>
		<button @click="primeiro($event), segundo($event)">Multiplos Eventos</button>
		<p>{{multiplosEventos}}</p>
	</div>
</template>
<script>
	export default{
		nome: 'multiplosEventos',
		data(){
			return{
				multiplosEventos: ""
			}
		},
		methods:{
			primeiro(event){
				this.multiplosEventos = "primeiro evento ativado"
			},
			segundo(event){
				setTimeout(()=> this.multiplosEventos = "segundo Evento ativado",  1000)
			}
		}
	}
</script>
<style scoped>
	div{
		margin: 100px
	}
</style>