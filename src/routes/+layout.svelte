<script>
	import '../app.css';
	let y;
	let navClass = '';

	function changeNav() {
		console.log('called');
		if (navClass == 'nav-scrolled') {
			navClass = '';
		} else if (navClass == '' && y > 0) {
			navClass = 'nav-scrolled';
		}
		return '';
	}
</script>

<svelte:window bind:scrollY={y} />

<nav id="nav" class="{navClass} nav-default">
	{#if y > 50}
		{changeNav()}
	{/if}

	{#if y < 50}
		{changeNav()}
	{/if}
	<div class="relative">
		<a
			class="font-roboto relative w-20 h-8 left-80 top-14 mr-20 font-bold text-2xl text-inherit hover:opacity-40 transition ease-linear duration-4000"
			href="#intro">INTRO</a
		>
		<a
			class="font-roboto relative w-20 h-8 left-80 top-14 mr-20 font-bold text-2xl text-inherit hover:opacity-40 transition ease-linear duration-4000"
			href="#resume">RESUME</a
		>
		<a
			class="font-roboto relative w-20 h-8 left-80 top-14 mr-20 font-bold text-2xl text-inherit hover:opacity-40 transition ease-linear duration-4000"
			href="#portfolio">PORTFOLIO</a
		>
		<a
			class="font-roboto relative w-20 h-8 left-80 top-14 mr-20 font-bold text-2xl text-inherit hover:opacity-40 transition ease-linear duration-4000"
			href="#contact">CONTACT</a
		>
	</div>
</nav>
<slot />

<style>
	.nav-scrolled {
		background-color: rgb(238, 224, 223);
		color: #555 !important;
		box-shadow: 0 5px 8px 0 rgba(0, 0, 0, 0.14);
		font-size: 1.875rem;
		position: fixed;
		width: 100%;
		overflow: hidden;
		height: 8rem;
		transition: none;
	}
	.nav-default {
		font-size: 1.875rem;
		line-height: 2.25rem;
		position: fixed;
		width: 100%;
		overflow: hidden;
		height: 8rem;
		color: white;
		z-index: 10;
		transition: all;
		transition-duration: 0.7s;
		-moz-transition: 0.32s;
		-moz-transition-timing-function: ease-in;
		transition-timing-function: ease;
	}
</style>
