<script>
	import '../app.css';
	import Nav from '$lib/components/Nav.svelte';
	import Dialog from '$lib/components//Dialog.svelte';

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

<header id="TopHeader">
	<div id="mobile-head">
		<button id="ToggleButton" class="btn" type="button" on:click={openDialog}>MENU</button>
		<Dialog bind:dialog on:closeDialog={closeDialog} />
	</div>
	<Nav />
</header>

<slot />
