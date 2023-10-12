<script>
	import { page } from '$app/stores';

	const pages = [
		{ name: 'Home', path: '/' },
		{ name: 'Profile', path: '/profile' },
		{ name: 'Contact', path: '/contact' }
	];
</script>

<nav id="global-nav">
	<ul>
		{#each pages as a}
			{#if a.path === $page.url.pathname}
				<li class="active"><a href={a.path}>{a.name}</a></li>
			{:else}
				<li><a href={a.path}>{a.name}</a></li>
			{/if}
		{/each}
	</ul>
</nav>

<style>
	a {
		text-decoration: none;
	}
	a:hover {
		filter: brightness(1.4); /* ホバー時に少し明るくする */
		text-decoration: underline;
	}
	.active a {
		color: #ff5722;
	}
</style>
