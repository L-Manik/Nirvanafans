<script lang="ts">
	import Section from '$components/Section.svelte';
	import book from 'svelte-awesome/icons/book';
	import music from 'svelte-awesome/icons/music';
	import cogs from 'svelte-awesome/icons/cogs';
	import user from 'svelte-awesome/icons/user';
	import Members from '$lib/components/Members.svelte';
</script>

<div class="readable-area">
	<div class="title">
		<header>
			<h1>Studio Albums Released by Nirvana</h1>
		</header>
	</div>

	<div class="albumsdisplay">
		<div class="album">
			<div class="info">
				<h1>Bleach</h1>
				<div class="desc">
					<p>
						"Bleach" is Nirvana's debut album, released in 1989. It features raw and aggressive
						songs, showcasing Kurt Cobain's gritty vocals and distorted guitar. While not
						commercially successful at the time, "Bleach" laid the foundation for Nirvana's later
						success and influenced the alternative music scene.
					</p>
				</div>
			</div>
			<div class="info">
				<iframe
					title="Bleach"
					style="border-radius:12px"
					src="https://open.spotify.com/embed/album/0CqchZDaOxckvjnKKfJh1w?utm_source=generator&theme=0"
					width="100%"
					height="352"
					frameBorder="0"
					allowfullscreen=""
					allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture"
					loading="lazy"
				/>
			</div>
		</div>
		<div class="album">
			<div class="info">
				<h1>Nevermind</h1>
				<div class="desc">
					<p>
						"Nevermind," released in 1991, is the groundbreaking second studio album by Nirvana.
						With the explosive anthem "Smells Like Teen Spirit" leading the way, the album
						revolutionized the music industry, introducing grunge to the mainstream. Its raw energy,
						introspective lyrics, and Kurt Cobain's distinctive vocals made "Nevermind" a cultural
						phenomenon, solidifying Nirvana's status as one of the most influential bands of all
						time. The album's impact continues to resonate, shaping alternative rock and inspiring
						countless musicians to this day.
					</p>
				</div>
			</div>
			<div class="info">
				<iframe
					title="Nevermind"
					style="border-radius:12px"
					src="https://open.spotify.com/embed/album/2UJcKiJxNryhL050F5Z1Fk?utm_source=generator"
					width="100%"
					height="352"
					frameBorder="0"
					allowfullscreen=""
					allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture"
					loading="lazy"
				/>
			</div>
		</div>
		<div class="album">
			<div class="info">
				<h1>In Utero</h1>
				<div class="desc">
					<p>
						"In Utero" is the third and final studio album by Nirvana, released in 1993. It
						represents a departure from the polished sound of their previous album, embracing a raw
						and abrasive sonic aesthetic. With tracks like "Heart-Shaped Box" and "All Apologies,"
						the album delves into darker and more introspective themes. "In Utero" showcases Kurt
						Cobain's raw songwriting and powerful vocals, capturing the band's raw energy and
						emotional intensity. While initially met with mixed reviews, the album has since been
						recognized as a significant artistic achievement, solidifying Nirvana's status as an
						influential force in alternative rock.
					</p>
				</div>
			</div>
			<div class="info">
				<iframe
					title="In Utero"
					style="border-radius:12px"
					src="https://open.spotify.com/embed/album/7wOOA7l306K8HfBKfPoafr?utm_source=generator"
					width="100%"
					height="352"
					frameBorder="0"
					allowfullscreen=""
					allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture"
					loading="lazy"
				/>
			</div>
		</div>
		<a class ="backbutton" href="/">Return</a>
	</div>
</div>

<style>
	.readable-area {
		padding: 5px;
		max-width: 960px;
		width: 95%;
		margin: 20px auto;
        background-color: black;
        border-radius: 3rem;
	}

	p {
		margin-left: 2rem;
	}
	.title {
		padding: 16px;
		display: flex;
		flex-direction: column-reverse;
		align-items: center;
		border-bottom: 4px solid black;
		text-decoration: none;
		color: #000000;
	}

	.info {
		display: flex;
		flex-direction: row;
		flex: 1;
	}

	.album {
		display: flex;
		flex-direction: column;
		flex: 1;
		gap: 16px;
		padding: 16px;
		border-radius: 10px;
		margin: 16px;
	}

	.album:nth-child(1) {
		border: white solid 5px;
		background-color: black;
	}

	.album:nth-child(2) {
		border: #1ccad8 solid 5px;
		background-color: #0167b2;
	}

	.album:nth-child(3) {
		border: #fdfbe6 solid 5px;
		background-color: #6b2b06  ;
        margin-bottom: 0.5rem;
	}

	
	.backbutton {
		margin-left: 2rem;
		margin-bottom: 3rem;
	}

</style>
