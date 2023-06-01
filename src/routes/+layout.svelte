<svelte:head>
	<link rel="preconnect" href="https://fonts.googleapis.com" />
	<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="anonymous" />
	<link
		href="https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;500&family=Peralta&display=swap"
		rel="stylesheet"
	/>
	<title>Svelte Spongebob CV</title>
	<script src="https://kit.fontawesome.com/5bb4fcfd58.js" crossorigin="anonymous"></script>
	<meta name="viewport" content="width=device-width, initial-scale=1" />
</svelte:head>

<slot />

<style>
	:global(*) {
		margin: 0;
		padding: 0;
		font-family: 'Open Sans';
		color: #e3e5f2;
		box-sizing: border-box;
	}
	:global(html, body) {
		width: 100%;
		height: 100%;
		/*background: repeating-linear-gradient(#101223, #09104d);*/
		background-image: radial-gradient(
			circle at top right,
			#101223 0%,
			#101223 48%,
			#090f4b 48%,
			#090f4b 53%,
			#030c5f 53%,
			#030c5f 56%,
			#030c5f 56%,
			#020f87 69%,
			#020f87 69%,
			#020f87 100%
		);
	}
	:global(a) {
		text-decoration: none;
	}

	@media (max-width: 768px) {
		:global(html, body) {
			width: 100%;
			height: 100%;
			background: #09104d;
		}
	}
</style>
