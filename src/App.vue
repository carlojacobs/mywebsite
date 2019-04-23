<template>
  <div id="app">
  	<Headers :colorClass="colorClass" @change-color="changeColor" :color="color"/>
  	<Info/>
  	<Portfolio :colorClass="colorClass" @toggleModal="toggleModal"/>
  	<Technologies :colorClass="colorClass"/>
  	<Modals :modals="modals" :colorClass="colorClass" @toggleModal="toggleModal"/>
  	<Footer :colorClass="colorClass"/>
  </div>
</template>

<script>
import Info from './components/Info.vue'
import Modals from './components/Modals.vue'
import Portfolio from './components/Portfolio.vue'
import Technologies from './components/Technologies.vue'
import Headers from './components/Headers.vue'
import Footer from './components/Footer.vue'

// Css
import '../node_modules/bulma/css/bulma.min.css';
import '../node_modules/bulma-divider/dist/css/bulma-divider.min.css';
import '../node_modules/@fortawesome/fontawesome-free/css/all.min.css';

export default {
  name: 'app',
  components: {
    Info,
    Modals,
    Portfolio,
    Technologies,
    Headers,
    Footer
  },
  data() {
		return {
			modals: {1: false, 2: false, 3: false, 4: false, 5: false, 6: false},
			colorClass: "",
			color: ""
		}
	},
	methods: {
		toggleModal(modal) {
			this.modals[modal] = !this.modals[modal];
		},
		changeColor(color) {
			this.color = color;
			if (color == "Blue") {
				this.colorClass = "is-info";
			}
			if (color == "Yellow") {
				this.colorClass = "is-warning";
			}
			if (color == "Red") {
				this.colorClass = "is-danger";
			}
			if (color == "Green") {
				this.colorClass = "is-success";
			}
		}
	},
	created() {
		var possibleColors = [["Yellow", "is-warning"], ["Green", "is-success"], ["Red", "is-danger"], ["Blue", "is-info"]]
		var randomIndex = Math.floor(Math.random() * possibleColors.length);
		this.color = possibleColors[randomIndex][0]
		this.colorClass = possibleColors[randomIndex][1]
	}
}
</script>

<style>
	body {
		font-family: 'Lato', sans-serif;

	}
</style>