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
						      <div class="media-left">
						        <figure class="image profile-figure is-96x96">
						          <img src="@/assets/profile.jpg" alt="me" class="profile-image">
						        </figure>
						      </div>
						      <div class="media-content">
						        <p class="title is-4 media-content-titles" style="margin: 0;">Carlo Jacobs</p>
						        <p class="media-content-titles">Hello World!</p>
						        <div class="buttons">
										  <a href="https://github.com/carlojacobs" class="button is-outlined" :class="colorClass"><span class="icon is-small"><i class="fab fa-github"></i></span><span>GitHub</span></a>
										  <a href="https://worldofscience.ml" class="button is-outlined" :class="colorClass">Latest project</a>
										  <a href="https://carlo-jacobs.com/blog" class="button is-outlined" :class="colorClass">Blog</a>
										</div>
						      </div>
						    </div>

						    <div class="content">
						      <p>My favourite quote: "One day I will find the right words, and they will be simple" - Jack Kerouac</p>
						      I'm an Active coder, problem solver and phycisist.
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
	.profile-figure {
		width: 10rem;
		height: 10rem;
		border-radius: 100%;
	}
	.profile-image {
		border-radius: 5px;
	}
	.media-content-titles {
		color: black !important;
	}
</style>
