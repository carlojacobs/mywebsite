<template>
	<section class="section hero is-dark"">
			<div class="container">
				<h1 class="title is-3">What have I made so far?</h1>
				<h3 class="subtitle is-4">I have built a couple of projects that actually made it to production. More can be found on my <a href="https://github.com/carlojacobs"><u>Github</u></a>.</h3>
				<div class="columns" v-for="row in projects">
					<div class="column portfolio-column" v-for="project in row">
						<div class="hero is-bold portfolio-item" :class="colorClass" v-on:click="toggleModal(project.modalId)">
							<p class="title">{{project.title}}</p>
							<p class="subtitle">{{project.subtitle}}</p>
						</div>
					</div>
				</div>
			</div>
		</section>
</template>

<script>
	export default {
		name: 'Portfolio',
		props: ['colorClass'],
		data() {
			return {
				projects: [
				[
					{
						title: "World of Science",
						subtitle: "World of Science is a place where people can learn about science.",
						size: "",
						modalId: 2
					}
				],
				[
					{
						title: "Tutoring Business Website",
						subtitle: "A website I created for my local tutoring business",
						size: "",
						modalId: 6
					},
					{
						title: "Titanic Predictor",
						subtitle: "I built a neural network that predicts if you would have survived the Titanic disaster.",
						size: "",
						modalId: 1
					},
					{
						title: "This website",
						subtitle: "I built this website using VueJS, HTML and CSS",
						size: "",
						modalId: 3
					}
				],
				[
					{
						title: "Game of Life",
						subtitle: "A python version of John Conway's Game of Life",
						size: "",
						modalId: 4
					},
					{
						title: "Classify",
						subtitle: "A place for students to share information",
						size: "",
						modalId: 5
					}
				],
				]
			}
		},
		methods: {
			toggleModal(modal) {
				this.$emit('toggleModal', modal);
			}
		}
	}
</script>

<style>
.portfolio-item {
	cursor: pointer;
	transition: .1s;
	/*border: 2px solid white;*/
	border-radius: 5px;
	height: 100%;
	/*padding: 2rem;*/
	padding: 1.25rem 2.5rem 1.25rem 1.5rem;
}
.portfolio-column:hover .portfolio-item,
.portfolio-column:focus .portfolio-item {
	transform: scale(0.95);
	transition-delay: .05s;
}
</style>