<template>
	<nav class="nav">
		<div class="logo">
			<img src="/src/assets/logo 1.svg" alt="logo">
			<p>Personal</p>
		</div>

  	<div class="menu">
			<p><a href="#" class="link">Обо мне</a></p>
			<p><a href="#" class="link">Навыки</a></p>
			<p><a href="#" class="link">Проекты</a></p>
			<p><a href="#" class="link">Контакты</a></p>
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
}
.menu{
	display: flex;
	font-weight: 600;
	gap: 32px;
	font-size: 24px;
}

.logo{
	display: flex;
	font-weight: 700;
	align-items: center;
	gap: 12px;
	font-family: "Sora", sans-serif;
	font-size: 24px;
}
.link{
	position: relative;

	

	&::after{
		content: '';
		position: absolute;
		top: 100%;
		left: 50%;
		translate: -50%;
		width: 0;
		height: 2px;
		background-color: currentColor;
		transition-duration: 0.2s;
	}
	&:hover{
		&::after{
			width: 100%;
		}
	}
}

</style>
