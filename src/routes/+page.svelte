<!-- opening part -->
<div class="readable-area">
	<a class="header" href="./photo.html">
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
		<div class="content-column">
			<div class="section-title">
				<i class="fa-solid fa-user title-icon" />
				Profile
			</div>
			<p>LOREM IPSUM</p>
			<div class="section-title">
				<i class="fa-solid fa-book title-icon" />
				Education
			</div>
			<ul>
				<li>
					<span>2011 - 2014</span>
					<span class="place">Bikini Bottom High School</span>
				</li>
				<li>
					<span>2011 - 2014</span>
					<span class="place">Bikini Bottom High School</span>
				</li>
			</ul>
		</div>
		<div class="content-column">
			<div class="section-title">
				<i class="fa-solid fa-user title-icon" />
				Education
			</div>
			<ul>
				<li>
					<span>2011 - 2014</span>
					<span class="place">Bikini Bottom High School</span>
				</li>
				<li>
					<span>2011 - 2014</span>
					<span class="place">Bikini Bottom High School</span>
				</li>
			</ul>
			<div class="section-title">
				<i class="fa-solid fa-wand-sparkles title-icon" />
				Skills
			</div>
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
		</div>
	</div>
</div>

<style>
	.readable-area {
		display: flex;
		flex-direction: column;
		background-color: #ffffff;
		margin: 0 15%;
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
		flex-direction: row;
		padding: 16px;
		justify-content: end;
		align-items: center;
		border-bottom: 4px solid #000000;
		text-decoration: none;
	}

	.header-text {
		text-align: end;
		margin-right: 16px;
	}

	/* container */
	.content {
		display: flex;
		flex-direction: row;
	}

	.content-column {
		flex: 1;
		padding: 0px 16px 16px 16px;
		background-color: white;
	}

	.section-title {
		background-color: #ffeb3b;
		border-left: solid 4px #fbc02d;
		padding: 8px 16px;
		text-transform: UPPERCASE;
		font-weight: 500;
		margin: 16px 0px;
	}

	.title-icon {
		margin-right: 8px;
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

	@media (max-width: 600px) {
		.readable-area {
			margin: 0 5%;
		}

		.header {
			flex-direction: column-reverse;
		}

		.header-text {
			text-align: center;
		}

		.content {
			flex-direction: column;
		}
	}
</style>
