<script>
	import '../app.css';
	import logo from '$lib/assets/logo1.svg';
	import Nav from '$lib/components/Nav.svelte';
	import Dialog from '$lib/components//Dialog.svelte';
	import { onMount, onDestroy } from 'svelte';

	const scrollNavBar = 50;
	let show = false;
	onMount(() => {
		window.onscroll = () => {
			if (window.scrollY > scrollNavBar) {
				show = true;
			} else {
				show = false;
			}
		};
	});

	/**
	 * @type {{ showModal: () => void; addEventListener: (arg0: string, arg1: (event: any) => void) => void; close: () => void; }}
	 */
	let dialog;

	function openDialog() {
		dialog.showModal();
		dialog.addEventListener('click', function (event) {
			if (event.target === dialog) {
				dialog.close();
			}
		});
	}

	function closeDialog() {
		dialog.close();
	}
</script>

<header id="TopHeader" class:fixed={show}>
	<div id="mobile-head">
		<a class="brand" href="/"><img alt="logo" src={logo} /></a>
		<button id="ToggleButton" class="btn" type="button" on:click={openDialog}>MENU</button>
		<Dialog bind:dialog on:closeDialog={closeDialog} />
	</div>
	<Nav />
</header>

<slot />
