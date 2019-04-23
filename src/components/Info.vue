<template>
	<section class="hero" :class="colorClass">
		<div class="hero-body">
			<div class="container">
				<h3 class="title is-3">I love to build things, solve problems and most importantly, to learn.</h3>
  			<div class="is-divider"></div>
				<div class="columns">
					<div class="column">
						<h1 class="title">Who am I?</h1>
						<h5 class="subtitle is-5">Hi there! My name is Carlo Jacobs, I am a student in the Netherlands and I am 16 years old. When I was around 10 years old, I discovered the world of programming. Since then, I have gained skills in many areas of the field. I learnt how to work with several languages, frameworks and other technologies. These skills have helped me build cool things such as webapps and neural networks.</h5>
					</div>
					<div class="column">
						<h1 class="title">My Programming Journey</h1>
						<h5 class="subtitle is-5">I got introduced to programming when I was around 10 years old. Around this time, I played around with some basic <b>HTML</b> and <b>CSS</b>, it wasn't much, but it was a start. About a year later, I started learning <b>Pyhton</b>. I loved the functionality and versatility of the language and quickly got fascinated with Machine Learning. In the mean time, I had gotten pretty good at <b>JavaScript</b> as well and started building web applications using <b>React</b> and <b>Vue</b> to build fast UI's. As well as <b>NodeJS</b> coupled with <b>ExpressJS</b> to build scalable API's.</h5>
					</div>
				</div>
			</div>
		</div>
	</section>
</template>

<script>
	export default {
		name: 'Info',
		props: ['colorClass']
	}
</script>