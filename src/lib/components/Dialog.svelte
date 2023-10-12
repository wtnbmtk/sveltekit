<script>
	import { page } from '$app/stores';
	import { createEventDispatcher } from 'svelte';

	const pages = [
		{ name: 'Home', path: '/' },
		{ name: 'About', path: '/about' },
		{ name: 'Blog', path: '/blog' }
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
			{#each pages as p}
				{#if p.path === $page.url.pathname}
					<p class="active"><a href={p.path}>{p.name}</a></p>
				{:else}
					<p><a href={p.path}>{p.name}</a></p>
				{/if}
			{/each}
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
