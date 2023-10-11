<script>
	import { fly, scale } from 'svelte/transition';
	import { quadOut } from 'svelte/easing';
	import { page } from '$app/stores';

	/**
	 * @type {any}
	 */
	export let open;

	const pages = [
		{ name: 'Home', path: '/' },
		{ name: 'About', path: '/about' },
		{ name: 'Blog', path: '/blog' }
	];
</script>

{#if open}
	<nav>
		{#each pages as p}
			{#if p.path === $page.url.pathname}
				<p class="active"><a href={p.path}>{p.name}</a></p>
			{:else}
				<p><a href={p.path}>{p.name}</a></p>
			{/if}
		{/each}
	</nav>

	<div class="bar" transition:scale={{ duration: 750, easing: quadOut, opacity: 1 }} />
{/if}

<style>
	:global(html) {
		background: white;
	}
	a {
		text-align: center;
		font-size: 1.5em;
		letter-spacing: 0.15em;
		padding: 1em 0;
		display: block;
		cursor: pointer;
		margin: auto;
		color: black;
		text-decoration: none;
	}
	a:hover {
		text-decoration: underline;
	}
	.bar {
		border-style: solid;
		border-color: black;
		border-width: 1px;
		height: 0;
	}
	.active {
		background-color: red;
	}
</style>
