<script>
	import { page } from '$app/stores';

	const pages = [
		{ name: 'Home', path: '/' },
		{ name: 'Profile', path: '/profile' },
		{ name: 'Contact', path: '/contact' },
		{ name: 'Infomation', path: '/information' }
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
<nav id="headerSNS">
	<ul>
		<li>
			<a href="https://www.instagram.com/wtnbmtk/"><i class="fa-brands fa-instagram fa-lg" /></a>
		</li>
		<li><a href="https://twitter.com/mtk754522/"><i class="fa-brands fa-twitter fa-lg" /></a></li>
		<li>
			<a href="mailto:wtnbmtk7@gmail.com"><i class="fa-sharp fa-solid fa-envelope fa-lg" /></a>
		</li>
	</ul>
</nav>

<style>
	a {
		text-decoration: none;
		display: inline-block;
		padding: 0 1rem;
		color: black;
	}
	a:hover {
		filter: brightness(1.4); /* ホバー時に少し明るくする */
		text-decoration: underline;
	}
	.active {
		background-color: black;
	}
	.active a {
		color: white;
	}
	#global-nav,
	#headerSNS {
		display: none;
		position: absolute;
	}
	#global-nav {
		inset: 0;
		margin: auto;
	}
	#global-nav ul {
		margin: 0;
	}
	#headerSNS {
		inset: 0 0 0 auto;
	}
	#headerSNS a {
		padding: 0 8px;
	}
	@media (width >= 800px) {
		#global-nav,
		#headerSNS {
			display: block;
			width: fit-content;
		}
		#global-nav ul li,
		#headerSNS ul li {
			display: inline-block;
		}
		#global-nav ul li {
			padding: 0 1rem;
		}
		#headerSNS ul li {
			padding-right: 8px;
		}
	}
</style>
