<script lang="ts">
	import Section from '$components/Section.svelte';
	import book from 'svelte-awesome/icons/book';
	import music from 'svelte-awesome/icons/music';
	import cogs from 'svelte-awesome/icons/cogs';
	import user from 'svelte-awesome/icons/user';
</script>

<head>
	<meta charset="utf-8" />
</head>

<div class="wrapper">
	<div class="header">
		<div class="logo">
			<img
				src="https://1000logos.net/wp-content/uploads/2017/03/Nirvana-Logo-1989.png"
				alt="logo"
				class="brandlogo"
			/>
		</div>
		<div class="more" />
		<a href="/membersRoute"class="redirects">Members</a>
		<div class="redirects">
			<p class="redirectdesc">Albums</p>
		</div>
		<div class="redirects">Merch</div>
	</div>
	<div class="slideshow">
		<img
			src="https://consequence.net/wp-content/uploads/2019/07/nirvana-live-loud-vinyl-streaming-release.png"
			alt="livephoto1"
			class="livephoto"
		/>
	</div>
</div>

<style>
	.wrapper {
		overflow-x: hidden;
	}

	.header {
		display: flex;
		flex-direction: columns;
		margin-right: 2rem;
		margin-top: 1rem;
	}

	.logo {
		flex: 1;
		padding: 1rem;
	}

	.brandlogo {
		max-width: 130px;
		border: 5px solid black;
		padding-left: 10px;
		padding-right: 10px;
		border-radius: 100px;
		background-color: black;
	}

	.more {
		display: flex;
		flex-direction: columns;
	}

	.redirects {
		margin: 1rem 1rem;
	}

	.redirects:hover {
		border-bottom: solid 3px white;
        transform:scale(1.1)
	}

    .livephoto {
        display:flex;
        justify-content: center;
        margin-top: 3rem;
		width: 100vw;
    }
</style>
