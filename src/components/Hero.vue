<template>
	<div class="container">
  <section class="hero">
		<div class="info">
			<div class="info-title">
				<p class="sora">Привет, Я <b>Алексей.</b></p>
				<p class="sora"><b>Frontend</b> <b class="text">Developer</b></p>
				<p class="sora">и UI/UX <b>Designer.</b></p>
			</div>

			<div class="info-main">
				<p>
					Я Алексей, фронтенд разработчик. 
					Умению работать в команде и коммуницировать с дизайнерами и бэкэнд разработчиками. Готов к обучению и освоению новых технологий. Мои главные качества: Внимание к деталям и креативный подход, 
					Способность решать проблемы и анализировать ошибки, Стремление к саморазвитию и профессиональному росту.
				</p>
			</div>
			<div class="icons">
				<a href="https://github.com/m1stens" target="_blank"><img src="/src/assets/GitHub.svg" alt="github"></a>
				<a href="https://discordapp.com/users/647432685014351874/" target="_blank"><img src="/src/assets/Discord.svg" alt="discord"></a>
				<a href="https://t.me/m1stens" target="_blank"><img src="/src/assets/Telegram.svg" alt="telegram"></a>
			</div>
		</div>
		<div class="image">
			<img src="/src/assets/Banner.svg" alt="banner">
			
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
	.hero{
		padding: 70px 0px;
		display: flex;
	}
	.icons{
		display: flex;
		gap: 32px;
		margin-top: 80px;
	}
	.info{
		max-width: 740px;
    padding-top: 110px;
	}
	.info-title {
		display: flex;
		font-size: 56px;
		letter-spacing: -2px;
		gap: 20px;
		line-height: 56px;
		flex-direction: column;
		
	}
	.text{
		
		text-shadow:
    -2px -2px 0 black,
    2px -2px 0 black,
    -2px 2px 0 black,
    2px 2px 0 black;
		color: white;
		
	}
	.info-main{
		margin-top: 28px;
		color: #71717A;
		font-size: 18px;
	}
	.image{
		position: absolute;
		z-index: 2;
		left: 740px;
	}

</style>
