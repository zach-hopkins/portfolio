<script async context="module">
	import '@fontsource/roboto-mono';
	import '@fontsource/roboto';
	import GithubIcon from '$lib/assets/github.svelte';
	import FacebookIcon from '$lib/assets/facebook.svelte';
	import LinkedinIcon from '$lib/assets/linkedin.svelte';
	import Headshot from '$lib/assets/headshot.svelte';
</script>

<main class="absolute z-0 text-[1.6rem] w-full font-roboto">
	<div
		class="absolute z-0 w-full h-[46.8rem] bg-no-repeat bg-cover"
		style="background-image: linear-gradient(54deg, rgba(74, 76, 179, 0.95) 34%, hsla(0, 34%, 71%, 0.95)),
	url('/texture.avif')"
	>
		<Headshot />
		<div class="relative w-max left-[58.1rem] top-20">
			<p
				class="relative w-max z-10 font-bold text-[4.4rem] leading-[5.8rem] top-[-32.5rem] h-8 items-center text-white"
			>
				Zach Hopkins_
			</p>
			<div
				class="relative w-max h-[3.8rem] z-10 font-semibold top-[-30.5rem] text-[1.6rem] leading-[5.8rem] items-center text-white"
			>
				<p>Full Stack Developer, Entrepreneur</p>
			</div>
			<br />
			<div
				class="about-normal relative w-[50rem] top-[-30.5rem] font-medium text-[1.6rem] leading-[3.8rem] items-center text-white"
			>
				<p class="text-white text-opacity-40">
					AGE:<span class="absolute left-40 text-white">26</span>
				</p>
				<p class="text-white text-opacity-40">
					PHONE:<span class="absolute left-40 text-white">+1 (800) 800-2321</span>
				</p>
				<p class="text-white text-opacity-40">
					EMAIL:<span class="absolute left-40 text-white">zh934@gmail.edu</span>
				</p>
				<p class="text-white text-opacity-40">
					AREA:<span class="absolute left-40 text-white">Phoenix, AZ</span>
				</p>
			</div>
			<div class="social-icons relative w-max top-[-27.5rem] flex flex-row">
				<a
					class="fill-white opacity-40 duration-500 mr-10 hover:fill-white hover:opacity-80"
					href="https://github.com/zach-hopkins"
					target="_blank"><GithubIcon /></a
				>
				<a
					class="fill-white opacity-40 duration-500 mr-10 hover:fill-white hover:opacity-80"
					href="https://www.linkedin.com/in/zachary-a-hopkins/"
					target="_blank"><LinkedinIcon /></a
				>
				<a
					class="fill-white opacity-40 duration-500 mr-10 hover:fill-white hover:opacity-80"
					href="https://www.facebook.com/zach.hopkins.391"
					target="_blank"><FacebookIcon /></a
				>
			</div>
		</div>
	</div>
	<div class="mt-[52.5rem] relative z-[-1] top-8 left-[18.3rem] w-max">
		<p
			class="intro-header typewriter font-medium text-[3.6rem] leading-[4.7rem] w-max text-gray-600"
		>
			Intro_
		</p>
		<div class="p-5" />
		<p
			class="relative text-[1.875rem] font-roboto font-light w-[95rem] text-gray-500 text-opacity-80"
		>
			Experienced full-stack developer and multi-founder. Worked in web and mobile app development,
			automation, and systems administration. Held leadership roles as President and CEO of multiple
			profitable ventures before discovering Web3 technologies and building out an arbitrage
			automation tool built purely in Python and generating $100K+ in monthly profits.
		</p>
	</div>
</main>

<style>
	:root {
		/* Production */
		font-size: 82.5%;
		/* Standard Base 10 (10px:1rem) */
		/* font-size: 62.5%; */
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
