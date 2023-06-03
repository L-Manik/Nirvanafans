<script lang="ts">
	import Section from '$components/Section.svelte';
	import book from 'svelte-awesome/icons/book';
	import music from 'svelte-awesome/icons/music';
	import cogs from 'svelte-awesome/icons/cogs';
	import user from 'svelte-awesome/icons/user';
	import Members from '$lib/components/Members.svelte';
</script>

<svelte:head>
	<title>Nirvana Members Bio</title>
</svelte:head>

<div class="readable-area">
	<div class="title">
		<header>
			<h1>Meet the Members of Nirvana!</h1>
			<a href="/" class="backbutton">Return</a>
		</header>
	</div>
	<div class="columns">
		<Members iconData={user} title="Kurt Cobain">
			<img
				src="https://pyxis.nymag.com/v1/imgs/52e/730/f379ef050c6acd9519c595544979a8072f-28-kurt-cobain.rsquare.w330.jpg"
				alt="Kurt Cobain"
			/>
			<div class="members-info">
				<p>
					Kurt Cobain started the grunge band Nirvana in 1988 and made the leap to a major label in
					1991, signing with Geffen Records. Cobain also began using heroin around this time. After
					releasing the highly successful album Nevermind, Nirvana's highly acclaimed album In Utero
					was released in 1993 and catapulted to the top of the music charts. On April 5, 1994, in
					the guest house behind his Seattle home, Cobain committed suicide.
				</p>
			</div>
		</Members>
		<Members iconData={user} title="Krist Novoselic">
			<img
				src="https://i.pinimg.com/736x/3d/11/83/3d1183ad687d9fb52d29e1c7967ea895.jpg"
				alt="Krist Novoselic"
			/>
			<div class="members-info">
				<p>
					Krist Novoselic, born in 1965, is the acclaimed bassist of Nirvana, helping shape their
					sound and pioneering the grunge movement alongside Kurt Cobain. Following Cobain's tragic
					death in 1994, Novoselic pursued various musical projects while maintaining a strong
					connection to Nirvana's legacy. His enduring impact in the alternative rock scene of the
					1990s continues to be widely recognized.
				</p>
			</div>
		</Members>
		<Members iconData={user} title="Dave Grohl">
			<img
				src="https://freshairarchive.org/sites/default/files/styles/square_1600/public/2021-08/DaveGrohl.jpg?itok=5k6UQ3yC"
				alt="Dave Grohl"
			/>
			<div class="members-info">
				<p>
					Musician Dave Grohl formed his first band at age 10. He dropped out of high school to play
					with the hardcore group Scream before auditioning for Nirvana. Nirvana went on to be an
					international hit. After singer Kurt Cobain's death, Grohl formed a commercially
					successful alternative band called the Foo Fighters.
				</p>
			</div>
		</Members>
	</div>
</div>

<style>
	.title {
		padding: 16px;
		display: flex;
		flex-direction: column-reverse;
		align-items: center;
		border-bottom: 4px solid black;
		text-decoration: none;
		color: #000000;
	}

	.readable-area {
		padding: 5px;
		max-width: 960px;
		width: 95%;
		margin: 20px auto;
	}

	header {
		padding: 0 15px;
		text-align: center;
		font-size: 21px;
	}

	.columns {
		display: flex;
		flex-flow: row wrap;
		justify-content: center;
		margin: 5px 0;
		gap: 16px;
	}

	img {
		width: 128px;
		height: 128px;
		border: 4px solid #000000;
		border-radius: 100%;
		display: block;
		margin-left: auto;
		margin-right: auto;
		margin-top: 16px;
		margin-bottom: 16px;
	}

	.backbutton:hover{
		border-bottom: white solid 2px;
	}

	@media (max-width: 768px) {
		.columns {
			display: flex;
			flex-flow: column;
			justify-content: center;
			margin: 5px 0;
			gap: 16px;
		}
	}
</style>
