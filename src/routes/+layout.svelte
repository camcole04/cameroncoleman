<script>
	import { onMount } from 'svelte';
	import MobileModal from '$lib/components/MobileModal.svelte';

	import assemblyLogo from '$lib/assets/language_logos/assembly.png';
	import cLogo from '$lib/assets/language_logos/C.png';
	import cssLogo from '$lib/assets/language_logos/CSS.png';
	import htmlLogo from '$lib/assets/language_logos/HTML.png';
	import javaLogo from '$lib/assets/language_logos/java.png';
	import jsLogo from '$lib/assets/language_logos/javascript.png';
	import pgLogo from '$lib/assets/language_logos/postgresql.png';
	import pythonLogo from '$lib/assets/language_logos/python.png';
	import svelteLogo from '$lib/assets/language_logos/svelte.png';

	let { children } = $props();

	const logos = [
		assemblyLogo,
		cLogo,
		cssLogo,
		htmlLogo,
		javaLogo,
		jsLogo,
		pgLogo,
		pythonLogo,
		svelteLogo
	];

	let logoInstances = $state([]);

	function randomInt(min, max) {
		return Math.floor(Math.random() * (max - min + 1)) + min;
	}

	onMount(() => {
		const instancesCount = 20;
		const logoWidth = 80;
		const logoHeight = 80;
		const placedLogos = [];

		function isOverlapping(x, y) {
			return placedLogos.some(pos => {
				return !(
					x + logoWidth < pos.x ||
					x > pos.x + logoWidth ||
					y + logoHeight < pos.y ||
					y > pos.y + logoHeight
				);
			});
		}

		const instances = [];

		for (let i = 0; i < instancesCount; i++) {
			let x, y;
			let attempts = 0;
			do {
				x = randomInt(0, 330 - logoWidth);
				y = randomInt(0, window.innerHeight - logoHeight);
				attempts++;
			} while (isOverlapping(x, y) && attempts < 100);

			placedLogos.push({ x, y });

			instances.push({
				src: logos[randomInt(0, logos.length - 1)],
				x,
				y,
				rotation: randomInt(0, 360)
			});
		}

		for (let i = 0; i < instancesCount; i++) {
			let x, y;
			let attempts = 0;
			do {
				x = randomInt(1700, window.innerWidth - logoWidth);
				y = randomInt(0, window.innerHeight - logoHeight);
				attempts++;
			} while (isOverlapping(x, y) && attempts < 100);

			placedLogos.push({ x, y });

			instances.push({
				src: logos[randomInt(0, logos.length - 1)],
				x,
				y,
				rotation: randomInt(0, 360)
			});
		}

		logoInstances = instances;
	});
</script>

<nav class="menu-nav">
	<h2 class="menu-header">QUICK LINKS</h2>
	<a class="menu-link" href="/" style="margin-bottom: 40px;">HOME</a>
	<a class="menu-link" href="/aboutme" style="margin-bottom: 40px;">ABOUT ME</a>
	<a class="menu-link" href="/#projects" style="margin-bottom: 40px;">PROJECTS</a>
</nav>

<div class="page-content">
	{@render children()}
</div>

<MobileModal />

<div class="background-logos">
	{#each logoInstances as logo}
		<img
			src={logo.src}
			alt="language logo"
			class="logo"
			style="top: {logo.y}px; left: {logo.x}px; transform: rotate({logo.rotation}deg);"
		/>
	{/each}
</div>

<style>
    @import '$lib/styles.css';

    .menu-nav {
        position: fixed;
        display: flex;
        flex-direction: column;
        background-color: #f5f1e9; /* light cream */
        padding: 40px 30px;
        height: 100vh;
        width: 10vw;
        box-shadow: 4px 0 10px rgba(0,0,0,0.1);
        border-right: 2px solid #d2b48c; /* tan for border */
        font-family: 'Georgia', serif;
        z-index: 10;
    }

    .menu-header {
        font-family: 'Palatino Linotype', 'Book Antiqua', Palatino, serif;
        /* font-size: 48px; */
		font-size: 2vw;
        color: #8b4513; /* brown */
        margin-bottom: 60px;
        text-align: center;
        letter-spacing: 3px;
        border-bottom: 2px solid #d2b48c;
        padding-bottom: 10px;
    }

    .menu-link {
        font-family: 'Georgia', serif;
        /* font-size: 28px; */
		font-size: 1.75vw;
        color: #5a3e1b; /* dark brown */
        text-decoration: none;
        margin-bottom: 30px;
        text-align: center;
        transition: color 0.3s ease;
    }

	/* @container sidebar (max-width: 10vw) {
		.menu-header {
			font-size: 2vw;
		}

		.menu-link {
			font-size: 3em;
		}
	} */

    .menu-link:hover {
        color: #a0522d; /* sienna */
        text-decoration: underline;
    }

	.background-logos {
		position: fixed;
		top: 0;
		/* left: 220px; start after menu */
		width: calc(100vw);
		height: 100vh;
		pointer-events: none;
		overflow: hidden;
		z-index: 0;
	}

	.background-logos .logo {
		position: absolute;
		width: 160px;
		height: 160px;
		/* filter: grayscale(100%); */
		opacity: 0.25;
		user-select: none;
		will-change: transform;
	}

	.page-content {
		position: relative;
		z-index: 2;
	}
</style>
