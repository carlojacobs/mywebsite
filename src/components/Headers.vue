<template>
	<section class="hero is-bold is-medium" :class="colorClass">
		<div class="hero-body">
			<div class="container header-container">
				<div class="columns">
					<div class="column">
						<h1 class="title is-1">My name is Carlo Jacobs.</h1>
						<h3 class="subtitle is-3">Need some code? Hit me up!</h3>
						<div class="field">
						  <label class="title is-6" for="color">Fancy some new colors?</label>
						  <div class="control">
						  	<div class="select">
							    <select id="color" name="color" class="is-medium" v-model="color" v-on:change="changeColor">
							      <option>Yellow</option>
							      <option>Blue</option>
							      <option>Green</option>
							      <option>Red</option>
							    </select>
								</div>
						  </div>
						</div>
					</div>
					<div class="column">
						<div class="card" style="border-radius: 5px;">
						  <div class="card-content">
						    <div class="media">
						      <div class="media-content">
						        <div class="buttons">
										  <a href="https://github.com/carlojacobs" class="button is-medium" :class="colorClass"><span class="icon is-small"><i class="fab fa-github"></i></span><span><b>GitHub</b></span></a>
										  <a href="https://carlo-jacobs.com/titanic" class="button is-medium" :class="colorClass"><b>Latest project</b></a>
										  <a href="https://carlo-jacobs.com/blog" class="button is-medium" :class="colorClass"><b>Blog</b></a>
										</div>
						      </div>
						    </div>

						    <div class="content">
						      <p>My favourite quote: "One day I will find the right words, and they will be simple" - Jack Kerouac</p>
						      I'm an active coder, problem solver and amateur phycisist.
						      <br>
						      <time datetime="2016-1-1">13:53 PM - 10 May 2002</time>
						    </div>
						  </div>
						</div>
					</div>
				</div>
			</div>
		</div>
	</section>
</template>

<script>
	export default {
		name: 'Headers',
		props: ['colorClass', 'color'],
		data() {
			return {
				navbarIsActive: false
			}
		},
		methods: {
			changeColor() {
				this.$emit('change-color', this.color);
			},
			toggleNav() {
				this.navbarIsActive = !this.navbarIsActive;
			}
		}
	}
</script>

<style>
	.profile-image {
		border-radius: 5px;
		transform: rotate(90deg);
		width: 100%;
		margin-top: 18%;
		vertical-align: middle !important;
	}
	.media-content-titles {
		color: black !important;
	}
</style>
