<template>
	<div>
		<!-- Modals -->
		<div class="modal" v-bind:class="{'is-active' : modals['1']}">
			<div class="modal-background"></div>
			<div class="modal-card">
				<header class="modal-card-head">
					<p class="modal-card-title">Titanic Predictor</p>
					<button class="delete" aria-label="close" v-on:click="toggleModal(1)"></button>
				</header>
				<section class="modal-card-body">
					<h1 id="machinelearningfromdisasterwouldyouhavesurvived" class="title is-3">Machine Learning from Disaster: Would You Have Survived?</h1>
					<p>In this project, I used machine learning to try and predict if a person was likely to survive the Titanic disaster. Using a dataset I obtained from <a href="https://www.kaggle.com/c/titanic">this kaggle competition</a>, I was able to train a simple neural network up to 94% accuracy. As a finishing touch, I built a neat little web-app around the model.</p>
					<br>
					<h2 id="tools" class="title is-3">Tools</h2>
					<p>For this project, I used <code>Python3</code>, my favourite language. In addition, I used several libraries for multiple purposes:</p>
					<br>
					<ol>
					    <li><a href="http://www.numpy.org/">Numpy</a> for linear algebra and other types of scientific computing.</li>
					    <li><a href="https://pandas.pydata.org/">Pandas</a> for data analysation and manipulation.</li>
					    <li><a href="https://www.tensorflow.org/">Tensorflow</a> for building the machine learing model.</li>
					    <li><a href="https://matplotlib.org/">Matplotlib</a> for visualizing and analysing data.</li>
					</ol>
					<br>
					<h2 id="example" class="title is-3">Current Status</h2>
          <p>You can find this project <a href="https://carlo-jacobs.com/titanic">here</a>.</p>
				</section>
				<footer class="modal-card-foot">
					<a href="https://github.com/carlojacobs/titanic" class="button is-medium" :class="colorClass">View on Github</a>
					<a href="https://carlo-jacobs.com/titanic" class="button is-dark is-medium">Visit Project</a>
				</footer>
			</div>
		</div>
		<div class="modal" v-bind:class="{'is-active' : modals['2']}">
			<div class="modal-background"></div>
			<div class="modal-card">
				<header class="modal-card-head">
					<p class="modal-card-title">World of Science</p>
					<button class="delete" aria-label="close" v-on:click="toggleModal(2)"></button>
				</header>
				<section class="modal-card-body">
					<h3 class="title is-3">World of Science</h3>
					<p>World of Science is an online science blog where people can learn and share  about the most interesting things in our universe.</p>
					<br>
					<h3 class="title is-3">Current status</h3>
					<p>This app is active and deployed, you can find it <a href="https://worldofscience.ml">here</a></p>
				</section>
				<footer class="modal-card-foot">
					<a href="https://github.com/carlojacobs/worldofscience" class="button is-medium" :class="colorClass">View on Github</a>
					<a href="https://worldofscience.ml" class="button is-dark is-medium">Visit Project</a>
				</footer>
			</div>
		</div>
		<div class="modal" v-bind:class="{'is-active' : modals['3']}">
			<div class="modal-background"></div>
			<div class="modal-card">
				<header class="modal-card-head">
					<p class="modal-card-title">This Website</p>
					<button class="delete" aria-label="close" v-on:click="toggleModal(3)"></button>
				</header>
				<section class="modal-card-body">
					<h3 class="title is-3">My personal website</h3>
					<p>This website was built with simplicity in mind. I like minimalism and a simple design. The website displays my information, a little bit of a backstory and my projects.</p>
					<br>
					<h3 class="title is-3">Tools</h3>
					<p>I built this website using a JavaScript library called <b>VueJS</b>. It's an awesome library that helps me build cool and fast UI's.</p>
					<br>
					<h3 class="title is-3">Current Status</h3>
					<p>You can find this website at <a href="https://carlojacobs.ga">www.carlojacobs.ga</a>.</p>
				</section>
				<footer class="modal-card-foot">
					<a href="https://github.com/carlojacobs/carlojacobs" class="button is-medium" :class="colorClass">View on Github</a>
					<a href="https://carlojacobs.ga" class="button is-dark is-medium">Visit Project</a>
				</footer>
			</div>
		</div>
		<div class="modal" v-bind:class="{'is-active' : modals['4']}">
			<div class="modal-background"></div>
			<div class="modal-card">
				<header class="modal-card-head">
					<p class="modal-card-title">Game of Life</p>
					<button class="delete" aria-label="close" v-on:click="toggleModal(4)"></button>
				</header>
				<section class="modal-card-body">
					<h1 id="johnconwaysgameoflife" class="title is-3">John Conway's Game of Life</h1>
					<p>This is a small project that I put together in <code>Python3</code>. It is a simulation of <a href="https://en.wikipedia.org/wiki/Conway%27s_Game_of_Life">John Conway's Game of Life</a>. This 'Game of Life' is a simple grid system containing 'active' and 'non-active' squares that evovle according to a specific set of rules:</p>
					<br>
					<ol>
					<li>Any live cell with fewer than two live neighbours dies, as if by underpopulation.</li>

					<li>Any live cell with two or three live neighbours lives on to the next generation.</li>

					<li>Any live cell with more than three live neighbours dies, as if by overpopulation.</li>

					<li>Any dead cell with exactly three live neighbours becomes a live cell, as if by reproduction.</li>
					</ol>
					<br>
					<p>With the help of <a href="https://matplotlib.org">Matplotlib</a> and <a href="https://numpy.org">Numpy</a> I was able to create a simple simulation of this game.</p>
					<br>	
					<h2 id="requirements" class="title is-3">Requirements</h2>
					<p>In order to run this program, you have to have the following installed on your computer.</p>
					<br>	
					<ol>
						<li><a href="https://www.python.org">Python3</a></li>
						<li><a href="https://matplotlib.org">Matplotlib</a></li>
						<li><a href="https://numpy.org">Numpy</a></li>
					<br>	
					</ol>
					<p>Run the program by running: <code>python3 gol.py</code>.</p>
				</section>
				<footer class="modal-card-foot">
					<a href="https://github.com/carlojacobs/gameoflife" class="button is-medium" :class="colorClass">View on Github</a>
				</footer>
			</div>
		</div>
		<div class="modal" v-bind:class="{'is-active' : modals['5']}">
			<div class="modal-background"></div>
			<div class="modal-card">
				<header class="modal-card-head">
					<p class="modal-card-title">Classify</p>
					<button class="delete" aria-label="close" v-on:click="toggleModal(5)"></button>
				</header>
				<section class="modal-card-body">
					<h1 id="classifywebapp" class="title is-3">Classify webapp</h1>
					<p>Classify is a web application that helps students communicate with each other in a structured way. You can make an account, create a class, add students to that class and share information with every student in the class.</p>
					<br>
					<h2 id="structure" class="title is-3">Structure</h2>
					<p>The web application consists of a front-end that is visible to the user, and a back-end that handles all data traffic between the database and the front-end. The front-end code can be found in the <a href="https://github.com/carlojacobs/classify/tree/master/client">client</a> folder.</p>
					<br>
					<h3 id="backend" class="title is-3">Back-end</h3>
					<p>The back-end was built using <a href="https://nodejs.org/en/">NodeJS</a>, a flexible framework that allows you to run <code>Javascript</code> on the serverside. In addition to <code>NodeJS</code>, I used a framework called <a href="https://expressjs.com/">Express</a>. Express is a lightweight framework for <code>NodeJS</code> that is perfect for building web-applications. Of course, every web-app needs a database to store its data. For this project I chose the <code>NoSQL</code> database [MongoDB] and its NodeJS client <a href="https://mongoosejs.com/">Mongoose</a>.</p>
					<br>
					<h3 id="frontend" class="title is-3">Front-end</h3>
					<p>In order to build the user interface of this web-app, I used <a href="https://reactjs.org/">React</a>. React is a JavaScript library for building user interfaces, created and maintained by Facebook. It allows you to break up the UI into re-useable classes called <code>Components</code>, these components make your web-app faster and more flexible.</p>
					<br>
					<p>Due to limited resources, this web-app is no longer online.</p>
				</section>
				<footer class="modal-card-foot">
					<a href="https://github.com/carlojacobs/classify" class="button is-medium" :class="colorClass">View on Github</a>
				</footer>
			</div>
		</div>
		<div class="modal" v-bind:class="{'is-active' : modals['6']}">
			<div class="modal-background"></div>
			<div class="modal-card">
				<header class="modal-card-head">
					<p class="modal-card-title">Tutoring Website</p>
					<button class="delete" aria-label="close" v-on:click="toggleModal(6)"></button>
				</header>
				<section class="modal-card-body">
					<h1 id="bijles" class="title is-3">Bijles</h1>
					<p>This is a site I built for my local tutoring business. It contains useful information about the business, as well as my contact information.</p>
					<br>
					<h2 id="tools" class="title is-3">Tools</h2>
					<p>This site was built using <code>HTML</code>, <code>CSS</code> and a JavaScript library called <code>React</code>.</p>
					<br>
					<h2 id="currentstatus" class="title is-3">Current Status</h2>
					<p>You can find this website <a href="https://bijlesdoorn.nl">here</a></p>
				</section>
				<footer class="modal-card-foot">
					<a href="https://github.com/carlojacobs/bijles" class="button is-medium" :class="colorClass">View on Github</a>
					<a href="https://bijlesdoorn.nl" class="button is-medium is-dark">Visit Project</a>
				</footer>
			</div>
		</div>
	</div>
</template>

<script>
	export default {
		name: 'Modals',
		props: {
			modals: Object,
			colorClass: String
		},
		methods: {
			toggleModal(modal) {
				this.$emit('toggleModal', modal);
			}
		}
	}
</script>

<style>
	ol, ul {
		margin-left: 1rem !important;
	}
</style>
