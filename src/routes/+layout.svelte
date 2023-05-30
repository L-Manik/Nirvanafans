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
		background: linear-gradient(45deg, #101223, #09104d);
	}
	:global(a) {
		text-decoration: none;
	}

</style>
