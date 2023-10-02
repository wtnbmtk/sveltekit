<script lang="ts">
	export let open = false;
</script>

<button class:open on:click={() => (open = !open)}>
	<svg width="40" height="40">
		<line id="top" x1="9" y1="10" x2="31" y2="10" />
		<line id="middle" x1="9" y1="20" x2="31" y2="20" />
		<line id="bottom" x1="9" y1="30" x2="31" y2="30" />
	</svg>
</button>

<style>
	button {
		display: inline-block;
		width: 40px;
		height: 40px;
		padding: 0;
		cursor: pointer;
		border: none;
		background: #333;
		box-shadow: inset 0 0 0 2px #cccccc; /* 内側に枠を付ける */
		z-index: 20; /* （これは必要に応じて）他の要素より上に表示する */
	}

	button:hover {
		background: #555;
	}

	svg line {
		stroke: currentColor;
		stroke-linecap: round;
		stroke-width: 3;
		stroke: #cccccc;
		transition: transform 0.2s ease-in-out;
	}

	.open #top {
		transform: translate(13px, -1px) rotate(45deg);
	}

	.open #middle {
		opacity: 0;
	}

	.open #bottom {
		transform: translate(-15px, 13px) rotate(-45deg);
	}
</style>
