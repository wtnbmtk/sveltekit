<script>
	import '../app.css';
	import logo_webp from '$lib/assets/black.webp';
	import logo_png from '$lib/assets/black.png';
	import Nav from '$lib/components/Nav.svelte';
	import Dialog from '$lib/components//Dialog.svelte';

	// @ts-ignore
	import Headroom from 'svelte-headroom';

	const onPin = () => console.log('pin');

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

<div id="headroom">
	<Headroom on:pin={onPin} duration="350ms" offset={50} tolerance={0}>
		<header>
			<a class="brand" href="/">
				<picture>
					<source srcset={logo_webp} type="image/webp" />
					<img src={logo_png} alt="logo" width="100" height="15" />
				</picture></a
			>
			<button class="btn" type="button" on:click={openDialog}>MENU</button>
			<Nav />
		</header>
	</Headroom>
</div>
<Dialog bind:dialog on:closeDialog={closeDialog} />

<slot />

<footer>
	<section id="sns" class="contents">
		<div>
			<nav id="under-nav">
				<ul>
					<li class="link1">
						<a href="https://lin.ee/VTOX579">LINE</a>
					</li>
					<li class="link2">
						<a href="https://twitter.com/webdachi">𝕏</a>
					</li>
				</ul>
			</nav>
		</div>
	</section>
	<small class="copyright">© 2023 Webdachi</small>
</footer>

<style>
	.brand {
		display: inline-block;
		margin-left: 16px;
	}

	@media (width >= 800px) {
		.btn {
			display: none;
		}
	}
</style>
