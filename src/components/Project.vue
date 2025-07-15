<template>
  
	<section class="project">
		<div class="sora title">
			<p>Мои <b>Проекты</b></p>
		</div>

		<div class="project-list">

			<div class="project-item">
				<div class="project-image">
					<img src="/src/assets/Cover.svg" alt="project" style="border-radius: 19px;">
				</div>
				<div class="project-info">
					<p class="sora number">
						<b>01</b>
					</p>
					<p class="sora title-project">
						Landing Positivus
					</p>
					<p class="main-info">
						Это агентство цифрового маркетинга, которое помогает компаниям расти и добиваться успеха в Интернете с помощью ряда услуг, включая SEO, PPC, маркетинг в социальных сетях и создание контента.
					</p>
					
					<a href="https://m1stens.github.io/positivus-main/" target="_blank" style="width: 20px;"><img src="/src/assets/Read More.svg" alt="Read More" style="width: 20px; height: 20px;" class="readMore"></a>
				</div>
			</div>

			<div class="project-item special">
				
				<div class="project-info special-info">
					<p class="sora number">
						<b>02</b>
					</p>
					<p class="sora title-project">
						Landing Fitness
					</p>
					<p class="main-info">
						Фитнес клуб "Kropp" — это современное пространство для тех, кто стремится к здоровому образу жизни и активному отдыху. Мы предлагаем широкий спектр услуг, которые подходят как новичкам, так и опытным спортсменам.
					</p>
					<a href="https://m1stens.github.io/kropp-fitness-main/" target="_blank" style="width: 20px;"><img src="/src/assets/Read More.svg" alt="Read More" style="width: 20px; height: 20px;" class="readMore"></a>
				</div>
				<div class="project-image special-image">
					<img src="/src/assets/Fitnes.svg" alt="project" style="border-radius: 19px;">
				</div>
			</div>

			<div class="project-item">
				<div class="project-image">
					<img src="/src/assets/Burger.svg" alt="project" style="border-radius: 19px;">
				</div>
				<div class="project-info">
					<p class="sora number">
						<b>03</b>
					</p>
					<p class="sora title-project">
						<b>Fast Food	</b>
					</p>
					<p class="main-info">
						Fast Food - представляет собой удобную платформу, которая позволяет пользователям заказывать блюда из любимых ресторанов с минимальными усилиями. 
						Веб-ресурс нацелен на оптимизацию процесса выбора, оплаты и доставки еды, предоставляя высокий уровень сервиса и разнообразие гастрономических предложений.
						
					</p>
					<a href="https://m1stens.github.io/WEB-PRO-Burger-Landing-FINAL/" target="_blank" style="width: 20px;" ><img src="/src/assets/Read More.svg" alt="Read More" style="width: 20px; height: 20px;" class="readMore"></a>
				</div>
			</div>

		</div>
	</section>

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
.project{
	padding: 60px 0px;
  align-items: center;
	background-color: black;
	margin-inline: auto;
	padding-inline: 275px;
}
.project-list{
	display: flex;
	color: white;
	flex-direction: column;
	gap: 45px;
	margin-top: 30px;
}
.project-item{
	display: flex;
	gap: 80px;
}
.project-image{
	padding: 20px 0px;
}
.project-info{
	display: flex;
	flex-direction: column;
	max-width: 700px;
	padding: 60px 0px;
	gap: 25px;
}
.number{
	font-size: 56px;
	line-height: 64px;
	
}
.title-project{
	font-size: 40px;
	line-height: 48px;
	font-weight: bold;
}
.main-info{
	font-size: 18px;
	line-height: 26px;
}
.title{
	color: white;
	font-size: 56px;
	line-height: 64px;
	text-align: center;
	padding: 20px 0px;
}
.readMore{
position: relative;

	&:hover{
		scale: 1.2;
		transition-duration: 0.2s;
		
	}
}
@media(max-width: 767px){
		.project{
			padding-inline: 20px;
		}
		.project-list{
			display: grid;
		}
		.project-item{
			display: grid;
			gap: 20px;
		}
		.project-info{
			padding: 20px 0px;
		}

		.special{
			grid-template-areas: 
			"image"
			"info"
			;
		}
		.special-info{
			grid-area: info;
		}
		.special-image{
			grid-area: image;
		}
	}
</style>
