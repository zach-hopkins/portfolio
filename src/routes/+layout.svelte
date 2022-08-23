<script>
	let y;
	let navClass = '';

	function changeNav() {
		if (navClass == 'nav-scrolled') {
			navClass = '';
		} else if (navClass == '' && y > 0) {
			navClass = 'nav-scrolled';
		}
		return '';
	}
</script>

<svelte:window bind:scrollY={y} />

<nav id="nav" class="nav {navClass}">
	{#if y > 1}
		{changeNav()}
	{/if}

	{#if y == 0}
		{changeNav()}
	{/if}

	<div class="links">
		<a href="#intro">INTRO</a>
		<a href="#resume">RESUME</a>
		<a href="#portfolio">PORTFOLIO</a>
		<a href="#contact">CONTACT</a>
	</div>
</nav>
<slot />

<style>
	.nav {
		font-size: 1.6rem;
		position: fixed;
		width: 100%;
		overflow: hidden;
		height: 7.8rem;
		color: #fff;
		transition: 0.35s;
	}
	.nav-scrolled {
		background-color: rgba(232, 217, 216);
		color: #555;
		box-shadow: 0 5px 8px 0 rgba(0, 0, 0, 0.14);
		/*copied*/
		font-size: 1.6rem;
		position: fixed;
		width: 100%;
		overflow: hidden;
		height: 7rem;
		transition: 0.5s;
	}
	.links {
		position: relative;
	}
	.links > a {
		text-decoration: none;
		position: relative;
		width: 4.7rem;
		height: 1.9rem;
		left: 20rem;
		top: 3.5rem;
		margin-right: 5rem;

		font-family: 'Roboto Mono', monospace;
		font-weight: 600;
		font-size: 1.4rem;
		line-height: 1.8rem;

		/* identical to box height */

		/* Nav Text */
		/*color: #555555;*/
		color: inherit;
	}
	.links > a:hover {
		opacity: 0.4;
	}
</style>
