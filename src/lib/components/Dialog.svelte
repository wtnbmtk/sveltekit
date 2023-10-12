<script>
	import { page } from '$app/stores';
	import { createEventDispatcher } from 'svelte';

	const pages = [
		{ name: 'Home', path: '/' },
		{ name: 'Profile', path: '/profile' },
		{ name: 'Contact', path: '/contact' }
	];

	export let dialog; // （←ポイント） 要素をバインドすることで親側で表示・閉じるの制御が可能に

	const dispatch = createEventDispatcher();
	function clickClose() {
		dispatch('closeDialog');
	}
</script>

<dialog bind:this={dialog}>
	<div class="inner">
		<h2>MENU</h2>
		<nav>
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
		<button class="close" on:click={clickClose}>CLOSE</button>
	</div>
</dialog>

<style>
	h2 {
		width: 100%;
		text-align: center;
	}
	a {
		display: block;
		color: black;
		text-decoration: none;
		text-align: center;
		margin: 0 4rem;
		cursor: pointer;
	}
	a:hover {
		text-decoration: underline;
	}
	.active {
		background-color: red; /* 赤い下線を引く */
	}
	.close {
		display: block;
		margin: 2rem auto 0;
		cursor: pointer;
	}
</style>
