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

		<div class="links">
			<a href="/membersRoute" class="redirects">Members</a>
			<a href="/albumsRoute" class="redirects">Albums</a>
			<a href="/merchRoute" class="redirects">Merch</a>
		</div>
	</div>
	<div id="slider">
		<figure>
			<img
				src="https://consequence.net/wp-content/uploads/2019/07/nirvana-live-loud-vinyl-streaming-release.png"
				alt="livephoto1"
				class="livephoto"
			/>
			<img
				src="https://m.media-amazon.com/images/M/MV5BMmMwZWQ5MGItYmY5My00NzU3LWIzZjMtNWU2ZDZkZjY3ZGJhXkEyXkFqcGdeQXVyMjUyNDk2ODc@._V1_.jpg"
				alt="livephoto1"
				class="livephoto"
			/>
			<img
				src="https://thumb.viva.co.id/media/frontend/thumbs3/2020/10/10/5f80ea0e21f05-viva-militer-sersan-satu-jason-everman-tengah-bersama-nirvana_1265_711.jpg"
				alt="livephoto1"
				class="livephoto"
			/>
			<img
				src="https://i.ytimg.com/vi/RLJLq8nqFsA/maxresdefault.jpg"
				alt="livephoto1"
				class="livephoto"
			/>
			<img
				src="https://consequence.net/wp-content/uploads/2019/07/nirvana-live-loud-vinyl-streaming-release.png"
				alt="livephoto1"
				class="livephoto"
			/>
		</figure>
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

	.links {
		margin-top: 1rem;
	}

	.redirects {
		margin: 1rem 1rem;
		margin-top: 1rem;
		padding-bottom: 8px;
	}

	.redirects:hover {
		border-bottom: solid 3px white;
		transform: scale(1.1);
	}

	.livephoto {
		display: flex;
		justify-content: center;
		width: 100vw;
	}

	#slider {
		overflow: hidden;
		background-color: black;
	}
	#slider figure {
		position: relative;
		width: 500%;
		margin: 0%;
		left: 0%;
		animation: 10s slider infinite;
	}
	#slider figure img {
		float: left;
		width: 20%;
	}
	@keyframes slider {
		0% {
			left: 0;
		}
		20% {
			left: 0;
		}
		25% {
			left: -100%;
		}
		45% {
			left: -100%;
		}
		50% {
			left: -200%;
		}
		70% {
			left: -200%;
		}
		75% {
			left: -300%;
		}
		95% {
			left: -300%;
		}
		100% {
			left: -400%;
		}
	}

	@media (max-width: 768px) {
		.header {
			display: flex;
			flex-direction: row;
			margin-right: 2rem;
			margin-top: 1rem;
		}
	}
</style>
