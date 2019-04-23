<template>
	<section class="section hero is-dark">
		<div class="container">
			<h1 class="title is-3">What I like to work with</h1>
			<h3 class="subtitle is-4">Over the years, my skills have developed a lot. This is what I like to work with the most.</h3>
			<div class="columns">
				<a href="https://vuejs.org" class="tech-a">
					<div class="column tech-column">
						<div class=" tech-box">
							<i class="fab fa-vuejs tech-fab" id="vue-fab"></i>
							<p> Vue.js is a library for building <b>interactive web interfaces</b>. The goal of Vue.js is to provide the benefits of reactive data binding and composable view components with an API that is as simple as possible.</p>
						</div>
					</div>
				</a>
				<a href="https://nodejs.org" class="tech-a">
					<div class="column tech-column">
						<div class=" tech-box">
							<i class="fab fa-node-js tech-fab" id="node-fab"></i>
							<p>Node.JS is a framework that turns <b>JavaScript</b> (the most popular programming language) into a <b>server side</b> language. Using Node.JS, I can build magnificent web applications, and complex API's that interact with <b>databases</b>.</p>
						</div>
					</div>
				</a>
				<a href="https://python.org" class="tech-a">
					<div class="column tech-column">
						<div class=" tech-box">
							<i class="fab fa-python tech-fab" id="python-fab"></i>
							<p>Python is the best programming language when it comes to <b>scientific computing</b>. Libraries like Tensorflow let me build complex neural networks and other <b>Artificial Intelligence (AI)</b> structures. This can be used for image recognition and other cool stuff!</p>
						</div>
					</div>
				</a>
				<a href="https://reactjs.org" class="tech-a">
					<div class="column tech-column">
						<div class=" tech-box">
							<i class="fab fa-react tech-fab" id="react-fab"></i>
							<p><b>React</b> is a framework built and maintained by Facebook. It was built to help us developers create powerful and beautiful user interfaces. It makes interacting with <b>API's</b> a lot easier and allows smooth flow of data.</p>
						</div>
					</div>
				</a>
			</div>
		</div>
	</section>
</template>

<script>
	export default {
		name: 'Technologies',
		props: ['colorClass']
	}
</script>

<style>
#vue-fab {
color: #42b883;
}

#node-fab {
  color: #6cc24a;
}

#python-fab {
  color: #4584b6;
}

#react-fab {
  color: #00d8ff;
}
.tech-a {
	color: black;
}
.tech-a:hover {
	color: black;
}
.tech-fab {
  font-size: 7rem;
}
.tech-column {
	text-align: center;
}
.tech-box {
	transition: .1s;
	border: none;
}
.tech-column:hover .tech-box,
.tech-column:focus .tech-box {
	transform: scale(0.95);
	transition-delay: .05s;
}
</style>