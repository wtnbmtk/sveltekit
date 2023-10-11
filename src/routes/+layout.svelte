<script>
	import Nav from '$lib/components/Nav.svelte';
	import Modal from '$lib/components/Modal.svelte';
	import { Hamburger } from 'svelte-hamburgers';
	import Menu from '$lib/components/Menu.svelte';
	/**
	 * @type {any}
	 */
	let open;
	let showModal = false;
</script>

<Nav />
<Hamburger bind:open --color="black" />
<Menu bind:open />

<button on:click={() => (showModal = true)} id="ToggleButton" class="btn" type="button"
	>MODAL</button
>

<Modal bind:showModal>
	<nav slot="nav" id="global-nav">
		<ul>
			<li><a class="list-1" href="#summary">概要</a></li>
			<li><a class="list-3" href="#profile">プロフィール</a></li>
			<li><a class="list-4" href="#contact">お問い合わせ</a></li>
		</ul>
	</nav>
</Modal>
<slot />
