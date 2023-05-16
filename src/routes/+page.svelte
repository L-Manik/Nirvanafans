<script lang="ts">
	import book from 'svelte-awesome/icons/book';
	import user from 'svelte-awesome/icons/user';
	import briefcase from 'svelte-awesome/icons/briefcase';
	import cogs from "svelte-awesome/icons/cogs";
	
	import Section from "$components/Section.svelte";
</script>

<!-- opening part -->
<div class="readable-area">
	<a class="header" href="./testRoute">
		<div class="header-text">
			<h1 class="name">Squarepants, Spongebob</h1>
			<p class="role">Head Chef</p>
		</div>
		<img
			src="https://assets.nick.com/uri/mgid:arc:imageassetref:nick.com:a625d441-bbbf-42c8-9927-6a0157aac911?quality=0.7"
			alt="Spongebob Profile"
		/>
	</a>
	<!-- first container -->
	<div class="content">
		<Section iconData={user} title="Profile">
				<p>LOREM IPSUN FOR THE WIN</p>
		</Section>
		<Section iconData={book} title="Education">
				<ul>
				<li>
					<span>2011 - 2014</span>
					<span class="place">Bikini Bottom High School</span>
				</li>
				<li>
					<span>2014 - 2016</span>
					<span class="place">McGuy University</span>
				</li>
				</ul>
		</Section>
		<Section iconData={briefcase} title="Job Experience">
				<ul>
					<li>
						<span>Burger Flipper (2017 - 2018)</span>
						<span class="place">Krusty Wrab</span>
					</li>
					<li>
						<span>Ministry of Defense (2018 - 2020)</span>
						<span class="place">Chum Bucket</span>
					</li>
				</ul>
		</Section>
		<Section iconData={cogs} title="Skills">
				<ul>
					<li class="skill">
						<span class="skill-title">Jellyfish Hunting</span>
						<div class="gauge">
							<div class="bullet filled-bullet" />
							<div class="bullet filled-bullet" />
							<div class="bullet filled-bullet" />
							<div class="bullet" />
							<div class="bullet" />
						</div>
					</li>
					<li class="skill">
						<span class="skill-title">Whale Singing</span>
						<div class="gauge">
							<div class="bullet filled-bullet" />
							<div class="bullet filled-bullet" />
							<div class="bullet" />
							<div class="bullet" />
							<div class="bullet" />
						</div>
					</li>
					<li class="skill">
						<span class="skill-title">Burger Flipping</span>
						<div class="gauge">
							<div class="bullet filled-bullet" />
							<div class="bullet filled-bullet" />
							<div class="bullet filled-bullet" />
							<div class="bullet filled-bullet" />
							<div class="bullet filled-bullet" />
						</div>
					</li>
				</ul>
		</Section>
	</div>
</div>

<style>
	.readable-area {
		display: flex;
		flex-direction: column;
		background-color: #ffffff;
		margin: 0 5%;
		height: 100%;
	}
    
	.name {
		font-family: 'Peralta', cursive;
		color: #000;
	}

	.role {
		font-weight: 500;
		color: #000;
	}

	img {
		width: 128px;
		height: 128px;
		border-radius: 100%;
		border: 4px solid #5e35b1;
	}

	.header {
		display: flex;
		flex-direction: column-reverse;
		padding: 16px;
		justify-content: end;
		align-items: center;
		border-bottom: 4px solid #000000;
		text-decoration: none;
	}

	.header-text {
		text-align: center;
		margin-right: 16px;
	}

	/* container */
	.content {
		display: grid;
		grid-template-columns: repeat(1, minmax(0, 1fr));
		gap: 2rem;
		padding: 2rem;
	}

	ul {
		list-style-type: none;
	}

	li {
		display: flex;
		flex-direction: column;
	}

	.place {
		margin-left: 16px;
	}

	.skill-title {
		flex: 1;
	}

	.gauge {
		display: flex;
		flex-direction: row;
		margin-left: 8px;
	}

	.bullet {
		width: 16px;
		height: 16px;
		border-radius: 100%;
		margin: 4px;
		background-color: #fff59d;
	}

	.filled-bullet {
		background-color: #fbc02d;
	}

	.skill {
		flex-direction: row;
		align-items: center;
		margin-bottom: 4px;
	}

	/* mobile first approach for future where there are more people using their phones */
	@media (min-width: 600px) {
		.readable-area {
			margin: 0 20%;
		}

		.header {
			flex-direction: row;
		}

		.header-text {
			text-align: end;
		}

		.content {
			grid-template-columns: repeat(2, minmax(0, 1fr))
		}
	}
</style>
