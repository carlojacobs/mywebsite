<template>
	<footer class="footer">
	  <div class="container">
	  	<h4 class="title is-4">Please feel free to write me a message!</h4>
	  	<form class="form-horizontal" action="https://formspree.io/carlormjacobs@gmail.com" method="POST">
				<fieldset>
					<div class="field">
					  <label class="label" for="name">Name</label>
					  <div class="control">
					    <input id="name" name="name" type="text" placeholder="Name..." class="input " required="">
					  </div>
					</div>
					<div class="field">
					  <label class="label" for="email">Email adress</label>
					  <div class="control">
					    <input id="email" name="_replyto" type="text" placeholder="Email..." class="input " required="">
					  </div>
					</div>
					<div class="field">
					  <label class="label" for="message">Message</label>
					  <div class="control">                     
					    <textarea class="textarea" id="message" name="message">Message...</textarea>
					  </div>
					</div>
					<div class="field">
					  <div class="control">
					  	<input type="submit" value="Send" class="button is-medium" :class="colorClass">
					  </div>
					</div>
				</fieldset>
			</form>
			<br>
			<p>This website was created and is being maintained by <a href="https://carlo-jacobs.com"a>Carlo Jacobs</a>.</p>
    	<br>
    	<small>&copy; Copyright 2019, Carlo Jacobs</small>
	  </div>
	</footer>
</template>

<script>
	export default {
		name: 'Footer',
		props: ['colorClass']
	}
</script>
