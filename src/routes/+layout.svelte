<script>
	import '../app.css';
	import logo_webp from '$lib/assets/logo1.webp';
	import logo_png from '$lib/assets/logo1.png';
	import Nav from '$lib/components/Nav.svelte';
	import Dialog from '$lib/components//Dialog.svelte';
	import { onMount } from 'svelte';

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
		<a class="brand" href="/">
			<picture>
				<source srcset={logo_webp} type="image/webp" />
				<img src={logo_png} alt="logo" width="100" height="100" />
			</picture></a
		>
		<button id="ToggleButton" class="btn" type="button" on:click={openDialog}>MENU</button>
		<Dialog bind:dialog on:closeDialog={closeDialog} />
	</div>
	<Nav />
</header>

<slot />
<a class="line" href="https://lin.ee/VTOX579"
	><img
		src="https://scdn.line-apps.com/n/line_add_friends/btn/ja.png"
		alt="友だち追加"
		height="36"
	/></a
>
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
