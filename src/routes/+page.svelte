<script async context="module">
	import '@fontsource/roboto-mono';
	import GithubIcon from '$lib/assets/github.svelte';
	import FacebookIcon from '$lib/assets/facebook.svelte';
	import LinkedinIcon from '$lib/assets/linkedin.svelte';
</script>

<main class="main">
	<div class="container">
		<img class="headshot" src="/headshot.avif" alt="headshot" />
		<div class="splash-text">
			<p class="about-header">Suri Ravi_</p>
			<div class="about-subheader">
				<p>Full Stack Developer, Entrepreneur</p>
			</div>
			<br />
			<div class="about-normal">
				<p>AGE:<span>26</span></p>
				<p>PHONE:<span>+1 (800) 800-2321</span></p>
				<p>EMAIL:<span>zh934@gmail.edu</span></p>
				<p>AREA:<span>Phoenix, AZ</span></p>
			</div>
			<div class="social-icons">
				<a href="https://github.com/zach-hopkins" target="_blank"><GithubIcon /></a>
				<a href="https://www.linkedin.com/in/zachary-a-hopkins/" target="_blank"><LinkedinIcon /></a
				>
				<a href="https://www.facebook.com/zach.hopkins.391" target="_blank"><FacebookIcon /></a>
			</div>
		</div>
	</div>
	<div class="intro">
		<p class="intro-header typewriter">Intro_</p>
	</div>
</main>

<style>
	:root {
		font-size: 62.5%;
		margin-left: -0.8rem;
	}
	.main {
		font-size: 1.6rem;
		position: absolute;
		width: 100%;
		z-index: -1;
	}
	.about {
		height: 54rem;
	}
	.container {
		position: absolute;
		z-index: -1;
		width: 100%;
		height: 46.8rem;
		margin-top: -0.82rem;
		background-image: linear-gradient(54deg, rgba(74, 76, 179, 0.95) 34%, hsla(0, 34%, 71%, 0.95)),
			url('/texture.avif');
		background-size: 100%;
		background-repeat: no-repeat;
	}
	.headshot {
		position: relative;
		width: 31.5rem;
		height: 38rem;
		left: 40rem;
		top: 11.7rem;
		z-index: 1;
		object-fit: cover;
		border-radius: 0.5rem;
		box-shadow: 0 0 27px rgba(96, 96, 96, 0.65);
	}
	.about-header {
		position: relative;
		width: max-content;
		height: 32px;
		left: 78.1rem;
		top: -32.5rem;
		z-index: 2;
		font-family: 'Roboto Mono', monospace;
		font-weight: 700;
		font-size: 4.4rem;
		line-height: 5.8rem;
		align-items: center;
		color: #fff;
	}
	.about-subheader {
		position: relative;
		width: max-content;
		height: 3.8rem;
		left: 78.1rem;
		top: -36.1rem;
		z-index: 2;
		font-family: 'Roboto Mono', monospace;
		font-weight: 600;
		font-size: 1.6rem;
		line-height: 5.8rem;
		align-items: center;
		color: #fff;
	}
	.about-normal {
		position: relative;
		width: 50rem;
		left: 78.1rem;
		top: -36.1rem;
		font-family: 'Roboto Mono', monospace;
		font-weight: 500;
		font-size: 1.6rem;
		line-height: 2.4rem;
		align-items: center;
		color: #fff;
	}
	.about-normal > p {
		color: rgba(255, 255, 255, 0.4);
	}

	.about-normal > p > span {
		position: absolute;
		left: 10rem;
		color: #fff;
		font-weight: normal;
	}

	.social-icons {
		position: relative;
		width: max-content;
		top: -34rem;
		left: 78.1rem;
	}
	.social-icons > a {
		margin-right: 2.4rem;
		fill: #fff;
		opacity: 0.4;
		transition: 0.5s;
	}
	.social-icons > a:hover {
		fill: #fff;
		opacity: 0.85;
	}

	.intro {
		display: absolute;
		margin-top: 55rem;
		z-index: -1;
	}

	.intro-header {
		display: inline-block;
		position: relative;
		font-family: 'Roboto Mono', monospace;
		font-weight: 500;
		font-size: 3.6rem;
		line-height: 4.7rem;
		padding-top: 2rem;
		padding-left: 38.3rem;
	}

	.typewriter {
		overflow: hidden; /* Ensures the content is not revealed until the animation */
		margin-top: 0.5rem;
		white-space: nowrap; /* Keeps the content on a single line */
		margin: 0 auto; /* Gives that scrolling effect as the typing happens */
		animation: typing 5.5s steps(150, end);
	}
	@keyframes typing {
		from {
			width: 0;
		}
		to {
			width: 100%;
		}
	}
</style>
