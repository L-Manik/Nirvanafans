<svelte:head>
	<link rel="preconnect" href="https://fonts.googleapis.com" />
	<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="anonymous" />
	<link
		href="https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;500&family=Peralta&display=swap"
		rel="stylesheet"
	/>
	<script src="https://kit.fontawesome.com/5bb4fcfd58.js" crossorigin="anonymous"></script>
	<meta name="viewport" content="width=device-width, initial-scale=1" />
</svelte:head>

<div class="main-wrapper">
	<div class="sidebar" />
	<div class="content">
		<slot />
	</div>
</div>

<style>
	:global(*) {
		margin: 0;
		padding: 0;
	}
	:global(html, body) {
		width: 100%;
		height: 100%;
	}
	.main-wrapper {
		width: 100%;
		height: 100%;
		display: flex;
		flex-direction: row;
	}
	.sidebar {
		background-color: blue;
		width: 200px;
		height: 100%;
	}
	.content {
		display: flex;
		flex-direction: column;
	}
</style>
