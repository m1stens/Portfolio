<template>
	<div class="container">
  <section class="talk">
		<form ref="myForm" @submit.prevent="submitForm" class="form">
			<input type="text" name="name" v-model="name" placeholder="Ваше имя" class="input">
			<input type="email" name="email" v-model="email" placeholder="Email" class="input">
			<input type="text" name="site" v-model="site" placeholder="Ваш сайт (Если есть)" class="input">
			<textarea name="help" id="help" v-model="message" placeholder="Как я могу помочь?" class="input textarea"></textarea>
			<div class="social">
				<button type="submit" class="submit">Связаться со мной</button>
				<div class="icons">
				<a href="https://github.com/m1stens" target="_blank"><img src="/src/assets/GitHub.svg" alt="github"></a>
				<a href="https://discordapp.com/users/647432685014351874/" target="_blank"><img src="/src/assets/Discord.svg" alt="discord"></a>
				<a href="https://t.me/m1stens" target="_blank"><img src="/src/assets/Telegram.svg" alt="telegram"></a>
				</div>
			</div>
		</form>
		<div class="info">
			<div class="main-text">
				<div class="sora">
					<p>Давайте <b class="text">поговорим</b>  </p>
					<p>О чем-то особенном</p>
				</div>
				<p class="stroke">Я стремлюсь расширить границы креативности, чтобы создавать увлекательные, удобные и запоминающиеся интерактивные проекты.</p>
			</div>
			<div class="contacts sora">
				<p>evseevalexej405@gmail.com</p>
				<p>89521104435</p>
			</div>
		</div>
	</section>	
</div>
</template>

<script >
const WEB3FORMS_ACCESS_KEY = "184b9d0b-5637-46ac-bb2a-51eb2f4c52e3";


export default {
	
	data() {
		return {
			name: "",
      email: "",
			site:"",
      message: "",


		}
	},
	
	methods: {
		async submitForm() {
        const response = await fetch("https://api.web3forms.com/submit", {
          method: "POST",
          headers: {
            "Content-Type": "application/json",
            Accept: "application/json",
          },
          body: JSON.stringify({
            access_key: WEB3FORMS_ACCESS_KEY,
            name: this.name,
            email: this.email,
						site: this.site,
            message: this.message,
          }),
        });
        const result = await response.json();
        if (result.success) {
          console.log(result);
        }
				this.$refs.myForm.reset()
      },
		
	},
	
}

</script>

<style scoped>
.talk{
	display: flex;
	padding: 60px 0px;
}
.form{
	display: flex;
	flex-direction: column;
	gap: 20px;
	padding: 20px 0px;
}
.input{
	width: 500px;
	padding: 18px 24px;
	font-size: 18px;
	line-height: 18px;
	border: 2px solid black;
	border-radius: 5px;

}
.textarea {
	height: 155px;
	font-size: 18px;
	line-height: 18px;
}
.submit{
	padding: 16px 20px;
	width: 230px;
	font-size: 20px;
	line-height: 20px;
	font-weight: 600;
	border: 2px solid black;
	border-radius: 5px;
	color: white;
	background-color: black;

	&:hover{
		opacity: 0.8;
		scale: 1.05;
		transition-duration: 0.2s;
	}
}
.social{
	display: flex;
		gap: 24px;
}
.icons{
		display: flex;
		gap: 24px;
		
	}
.info{
	display: flex;
	flex-direction: column;
	gap: 40px;
	padding: 20px 0px;
	max-width: 625px;
	margin-left: 220px;
}
.main-text{
	padding-top: 83px;
	display: flex;
	flex-direction: column;
	gap: 20px;

}
.main-text .sora{
	font-size: 56px;
	line-height: 56px;
	font-weight: 700;
	letter-spacing: -2px;
	display: flex;
	flex-direction: column;
	gap: 20px;
}
.text{
	text-shadow:
    -2px -2px 0 black,
    2px -2px 0 black,
    -2px 2px 0 black,
    2px 2px 0 black;
		color: white;
}
.stroke{
	font-size: 18px;
	line-height: 22px;
	color: #71717A;
	letter-spacing: 0px;
	font-weight: normal;
}
.contacts{
	font-size: 32px;
	line-height: 32px;
	font-weight: 600;
	display: flex;
	flex-direction: column;
	gap: 16px;
}
</style>
