<script>
	import { page } from '$app/stores';

	const pages = [
		{ name: 'Home', path: '/' },
		{ name: 'About', path: '/about' },
		{ name: 'Blog', path: '/blog' }
	];
</script>

<nav id="global-nav">
	{#each pages as p}
		{#if p.path === $page.url.pathname}
			<p class="active"><a href={p.path}>{p.name}</a></p>
		{:else}
			<p><a href={p.path}>{p.name}</a></p>
		{/if}
	{/each}
</nav>

<style>
	nav {
		display: flex;
		gap: 0.5rem;
	}

	a,
	p {
		color: white;
		background: #333;
		padding: 0.5em 1em;
		text-decoration: none;
	}

	a:hover {
		filter: brightness(1.4); /* ホバー時に少し明るくする */
		text-decoration: underline;
	}

	.active {
		box-shadow: 0 4px 0 0 red; /* 赤い下線を引く */
	}
</style>
