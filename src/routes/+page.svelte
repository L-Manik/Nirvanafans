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
	<div class="moreinfo">
		<div class="timeline">
			<div class="title">
				<h1>History of Nirvana</h1>
			</div>
			<div class="container left">
				<span class="dot-left" />
				<div class="text-box">
					<h2>Formation and Early Years</h2>
					<small
						>Nirvana was formed in 1987 in Aberdeen, Washington, by lead vocalist and guitarist Kurt
						Cobain and bassist Krist Novoselic. They went through several drummers before finally
						settling with Dave Grohl in 1990. The band quickly gained a reputation for their
						energetic live performances and distinctive sound, combining elements of punk, rock, and
						pop.</small
					>
				</div>
			</div>
			<div class="container right">
				<span class="dot" />
				<div class="text-box">
					<h2>Breakthrough with "Smells Like Teen Spirit"</h2>
					<small
						>In 1991, Nirvana released their second studio album, "Nevermind," which included the
						iconic single "Smells Like Teen Spirit." The song became an anthem for a disenchanted
						generation and propelled the album to immense commercial success. "Nevermind" topped
						charts worldwide and thrust Nirvana into the mainstream, marking the rise of the grunge
						movement and solidifying their status as one of the most important bands of the era.</small
					>
				</div>
			</div>
			<div class="container left">
				<span class="dot-left" />
				<div class="text-box">
					<h2>Follow-up Album "In Utero" and Tensions</h2>
					<small
						>Nirvana's third studio album, "In Utero," was released in 1993. It showcased a more raw
						and introspective side of the band's music. While critically acclaimed, tensions within
						the band began to surface. Kurt Cobain's struggles with drug addiction and his unease
						with fame added strain to the group's dynamics, but they embarked on a successful tour
						to support the album.</small
					>
				</div>
			</div>
			<div class="container right">
				<span class="dot" />
				<div class="text-box">
					<h2>Kurt Cobain's Tragic Suicide</h2>
					<small
						>On April 5, 1994, Kurt Cobain was found dead at his home in Seattle, Washington, having
						taken his own life. His death sent shockwaves through the music world and left fans
						devastated. Cobain's suicide marked the tragic end of Nirvana and left an irreplaceable
						void in the music industry. His profound influence as a songwriter and his troubled life
						have continued to captivate audiences even after his passing.</small
					>
				</div>
			</div>
			<div class="container left">
				<span class="dot-left" />
				<div class="text-box">
					<h2>Legacy and Cultural Impact</h2>
					<small
						>Despite their short-lived career, Nirvana's impact on music and popular culture cannot
						be overstated. Their music encapsulated the frustration and disillusionment of a
						generation, inspiring countless bands and shaping the alternative rock genre. Nirvana's
						discography, including iconic albums like "Nevermind" and "In Utero," remains widely
						celebrated. The band's cultural significance endures, as they are often credited with
						reshaping the trajectory of rock music in the early 1990s and leaving an indelible mark
						on the music industry.</small
					>
				</div>
			</div>
			<div class="end" />
		</div>
	</div>
</div>

<style>
	.wrapper {
		overflow-x: hidden;
		backdrop-filter: blur(50px);
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
		padding: 8px;
		background-color: rgba(0, 0, 0, 0.5);
		border-radius: 10px;
		transition: 0.005s;
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

	.moreinfo {
		display: flex;
		flex-direction: column;
		justify-content: center;
	}

	.title {
		background-color: #000000;
		padding: 2rem;
		border-radius: 15px;
		text-align: center;
	}

	.end {
		background-color: #000000;
		padding: 0.5rem;
		border-radius: 15px;
		text-align: center;
	}

	.timeline {
		position: relative;
		max-width: 1200px;
		margin: 100px auto;
	}

	.container {
		padding: 10px 50px;
		position: relative;
		width: 50%;
	}

	.left {
		left: 50%;
	}

	.dot-left {
		height: 40px;
		width: 40px;
		background-color: #000000;
		border-radius: 50%;
		display: inline-block;
		position: absolute;
		right: -20px;
		top: 32px;
		z-index: 10;
		left: -20px;
	}

	.text-box {
		padding: 20px 30px;
		background: #1c1d3c;
		position: relative;
		border-radius: 10px;
	}

	.dot {
		height: 40px;
		width: 40px;
		background-color: #000000;
		border-radius: 50%;
		display: inline-block;
		position: absolute;
		right: -20px;
		top: 32px;
		z-index: 10;
	}

	.timeline::after {
		content: '';
		position: absolute;
		width: 6px;
		height: 100%;
		background: #000000;
		top: 0;
		left: 50%;
		margin-left: -3px;
		z-index: -1;
	}

	@media (max-width: 768px) {
		.header {
			display: flex;
			flex-direction: row;
			margin-right: 2rem;
			margin-top: 1rem;
		}

		.links {
			display: column;
		}

		.timeline {
			margin: 50px auto;
		}

		.timeline::after {
			left: 31px;
		}

		.container {
			width: 100%;
			padding-left: 80px;
			padding-right: 25px;
		}

		.text-box {
			font-size: 13px;
		}

		.text-box small {
			margin-bottom: 10px;
		}

		.left {
			left: 0;
		}

		.dot,
		.dot-left {
			left: 10px;
		}
	}
</style>
