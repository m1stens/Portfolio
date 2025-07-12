<template>
  <div class="container">
		<section class="skills">
		<div class="title">
			<p class="sora">Мои <b>Навыки</b></p>
		</div>
		<div class="icons">
			
			<img src="/src/assets/HTML.svg" alt="HTML">
			<img src="/src/assets/Js.svg" alt="js">
			<img src="/src/assets/CSS.svg" alt="css">
			<img src="/src/assets/Sass.svg" alt="sass">
			<img src="/src/assets/Bootstrap.svg" alt="Bootstrap">
			<img src="/src/assets/Vue.svg" alt="vue">
			<img src="/src/assets/React.svg" alt="react">
			<img src="/src/assets/NodeJs.svg" alt="NodeJs">
			<img src="/src/assets/PHP.svg" alt="PHP">
			<img src="/src/assets/Git.svg" alt="git">
		</div>
	</section>
	</div>
	
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
.skills{
	display: flex;
	flex-direction: column;
  align-items: center;
	padding: 60px 0px;
}
.title{
	font-size: 56px;
    letter-spacing: -2px;
    
    line-height: 56px;
}

.icons{
	display: grid;
	grid-template-rows: 230px 186px;
  grid-template-columns: repeat(5, 186px);
  column-gap: 106px;
	margin-top: 75px;
}

</style>
