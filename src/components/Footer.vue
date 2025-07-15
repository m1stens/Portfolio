<template>
	<nav class="nav">
		<div class="logo">
			<img src="/src/assets/logo 2.svg" alt="logo">
			<p>Personal</p>
		</div>

  	<div class="menu">
			<p>@ 2025 Personal</p>
			
		</div>
  </nav>

</template>

<script >
export default {
	
	data() {
		return {


		}
	},
	
	methods: {
		
		
	},
	
}

</script>

<style scoped>

.nav{
	display: flex;
	justify-content: space-between;
	align-items: center;
	padding: 24px 275px;
	background-color: black;
}
.menu{
	display: flex;
	font-weight: 600;
	gap: 32px;
	font-size: 20px;
	color: white;
}

.logo{
	display: flex;
	font-weight: 700;
	align-items: center;
	gap: 12px;
	font-family: "Sora", sans-serif;
	font-size: 24px;
	color: white;
}
@media(max-width: 767px){
		.nav{
			padding: 24px 20px;
		}
	}


</style>
