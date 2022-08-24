<script async context="module">
	import '@fontsource/roboto-mono';
	import '@fontsource/roboto';
	import GithubIcon from '$lib/assets/github.svelte';
	import FacebookIcon from '$lib/assets/facebook.svelte';
	import LinkedinIcon from '$lib/assets/linkedin.svelte';
	import Headshot from '$lib/assets/headshot.svelte';
</script>

<main class="absolute z-[-1] text-[1.6rem] w-full font-roboto">
	<div
		class="absolute z-[-1] w-full h-[46.8rem] bg-no-repeat bg-cover"
		style="background-image: linear-gradient(54deg, rgba(74, 76, 179, 0.95) 34%, hsla(0, 34%, 71%, 0.95)),
	url('/texture.avif')"
	>
		<Headshot />
		<div class="splash-text">
			<p class="about-header">Zach Hopkins_</p>
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
		<p class="intro-body">
			Multi-founder, and experienced full-stack developer. Worked in web and mobile app development,
			automation, and systems administration. Held leadership roles as President and CEO of multiple
			profitable ventures before discovering Web3 technologies and building out an arbitrage
			automation tool built purely in Python and generating $100K+ in monthly profits.
		</p>
	</div>
</main>

<style>
	:root {
		/* Production */
		font-size: 62.5%;
		/* Standard Base 10 (10px:1rem) */
		/* font-size: 62.5%; */
		margin-top: -0.8rem;
		margin-left: -0.8rem;
	}
	.splash-text {
		position: relative;
		left: 58.1rem;
		width: max-content;
	}
	.about-header {
		position: relative;
		width: max-content;
		height: 32px;
		top: -32.5rem;
		z-index: 2;
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
		top: -35.1rem;
		z-index: 2;
		font-weight: 600;
		font-size: 1.6rem;
		line-height: 5.8rem;
		align-items: center;
		color: #fff;
	}
	.about-normal {
		position: relative;
		width: 50rem;
		top: -34.1rem;
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
		top: -32rem;
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
		margin-top: 52.5rem;
		position: relative;
		z-index: -1;
		top: 2rem;
		left: 18.3rem;
		width: max-content;
	}

	.intro-header {
		font-weight: 500;
		font-size: 3.6rem;
		line-height: 4.7rem;
		width: max-content;
		color: #555555;
	}

	.intro-body {
		position: relative;
		font-size: 1.8rem;
		line-height: 3rem;
		font-family: 'Roboto', sans-serif;
		font-weight: lighter;
		width: 90rem;
		color: rgba(85, 85, 85, 0.85);
	}

	.typewriter {
		overflow: hidden; /* Ensures the content is not revealed until the animation */
		margin-top: 0.5rem;
		white-space: nowrap; /* Keeps the content on a single line */
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
