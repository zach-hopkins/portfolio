<nav class="nav">
	<div class="links">
		<a href="#intro">INTRO</a>
		<a href="#resume">RESUME</a>
		<a href="#portfolio">PORTFOLIO</a>
		<a href="#contact">CONTACT</a>
	</div>
</nav>
<slot />

<style>
	:root {
		font-size: 62.5%;
	}
	.nav {
		font-size: 1.6rem;
		padding-left: 20rem;
		position: fixed;
		width: 144rem;
		height: 7rem;
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
		top: 2.5rem;
		margin-right: 5rem;

		font-family: 'Roboto Mono', monospace;
		font-weight: 600;
		font-size: 1.4rem;
		line-height: 1.8rem;

		/* identical to box height */

		/* Nav Text */
		/*color: #555555;*/
		color: #fff;
		transition: 0.2s;
	}
	.links > a:hover {
		opacity: 0.4;
	}
</style>
