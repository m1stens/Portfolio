<template>

  <header>
   <Head/>
  </header>

  <main>
		
    	<Hero/>
			<Skills/>
			<About/>
			<Project/>
			<Form/>
	
  </main>
	<footer>
		<Footer/>
	</footer>
	
</template>

<script >
import Head from './components/Head.vue';
import Hero from './components/Hero.vue';
import Skills from './components/skills.vue';
import About from './components/About.vue';
import Project from './components/Project.vue';
import Form from './components/Form.vue';
import Footer from './components/Footer.vue';
//import { RouterView } from 'vue-router';


export default {
	components: {Head, Hero, Skills, About, Project, Form, Footer},
	data() {
		return {


		}
	},
	
	methods: {
		
		
	},
	
}

</script>

<style scoped>

</style>
