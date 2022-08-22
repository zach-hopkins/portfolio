<script>
	import GithubIcon from '../lib/github.svelte';
	import FacebookIcon from '../lib/facebook.svelte';
	import LinkedinIcon from '../lib/linkedin.svelte';
</script>

<main class="main">
	<a id="about" class="about">
		<div class="container">
			<img class="headshot" src="/headshot.jpeg" alt="headshot" />
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
					<a href="" target="_blank"><GithubIcon /></a>
					<a href="" target="_blank"><LinkedinIcon /></a>
					<a href="" target="_blank"><FacebookIcon /></a>
				</div>
			</div>
		</div></a
	>
	<a id="intro" class="intro">
		<div class="hi">
			<p class="intro-header typewriter">Intro_</p>
		</div>
	</a>
</main>

<style>
	:root {
		font-size: 62.5%;
	}
	.main {
		font-size: 1.6rem;
		display: grid;
		position: absolute;
	}
	.about {
		padding-left: 20rem;
		height: 54rem;
	}
	.container {
		content: '';
		position: absolute;
		z-index: -1;
		width: 100vw;
		height: 46.8rem;
		margin-left: -21.6rem;
		margin-top: -0.82rem;
		background-image: url('/texture.jpg');
		background-size: cover;
		background-repeat: no-repeat;
	}
	.container::before {
		background: linear-gradient(54deg, rgba(74, 76, 179, 0.95) 34%, hsla(0, 34%, 71%, 0.95));
		content: '';
		z-index: 0;
		width: 215vh;
		height: 100%;
		position: absolute;
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
		width: auto;
		height: 32px;
		left: 78.1rem;
		top: -32.5rem;
		z-index: 2;
		font-family: 'Roboto Mono';
		font-weight: 500;
		font-size: 4.4rem;
		line-height: 5.8rem;
		align-items: center;
		color: #fff;
	}
	.about-subheader {
		position: relative;
		width: auto;
		height: 3.8rem;
		left: 78.1rem;
		top: -36.1rem;
		z-index: 2;
		font-family: 'Roboto Mono';
		font-weight: 500;
		font-size: 1.6rem;
		line-height: 5.8rem;
		align-items: center;
		color: #fff;
	}
	.about-normal {
		position: relative;
		width: auto;
		left: 78.1rem;
		top: -36.1rem;
		font-family: 'Roboto Mono';
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
	.hi {
		position: relative;
		display: inline-block;
	}
	.intro-header {
		display: inline-block;
		position: relative;
		font-family: 'Roboto Mono', monospace;
		font-weight: 400;
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
		animation: typing 1.5s steps(40, end);
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
