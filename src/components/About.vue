<template>
  <div class="container">
	<section class="about">
		<div class="about-image">
			<img src="/src/assets/About.svg" alt="about">
		</div>
		<div class="about-info">
			<p class="sora">Обо <b>Мне</b></p>
			<p>Я страстный, самопровозглашенный разработчик, специализирующийся на frontend разработке. 
				 Я с большим энтузиазмом отношусь к воплощению технических и визуальных аспектов цифровых продуктов в жизнь. 
				 Для меня важны пользовательский опыт, Pixel Perfect вёрстка и написание понятного, читаемого, высокопроизводительного кода.
			</p>
			<p>
				Я начал свой путь веб-разработчика в 2022 году, и с тех пор я продолжал расти и развиваться как разработчик, принимая новые вызовы и изучая новейшие технологии по пути. 
				Теперь я создаю передовые веб-приложения, используя современные технологии, такие как Vue.js, React.js, Bootstrap css и многое другое.
			</p>
			<p>
				Когда я не полностью занят разработкой, вы можете найти меня наблюдающим за развитием ранних стартапов или наслаждающимся свободным временем. 
				Вы можете следить за мной на GitHub.
			</p>
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
.about{
	display: flex;
	padding: 60px 0px;
	justify-content: space-between;
}
.about-info{
	max-width: 745px;
	font-size: 18px;
	color: #71717A;
}
.about-info p{
	margin-bottom: 20px;
}
.sora{
	font-size: 56px;
  padding-top: 20px;
	color: black;
}


</style>
