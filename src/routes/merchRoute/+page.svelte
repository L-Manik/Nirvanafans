<svelte:head>
	<title>Nirvana Merchandise</title>
</svelte:head>

<div class="readable-area">
	<div class="header">
		<img
			src="https://cdn.shopify.com/s/files/1/2081/4611/files/nirvana-logo_410x_f062795e-004e-4afd-8ba7-fc0160687616_700x.png?v=1631831561"
			alt="logo"
			class="brandlogo"
		/>
		<h1>Merchandise</h1>
		<a href="/">Return</a>
	</div>

	<div class="content">
		<div class="merchlist">
			<div class="merch">
				<a href="https://shop.nirvana.com/products/gritty-nevermind-hoodie?_pos=1&_sid=29c2c8a64&_ss=r">Gritty Nevermind Hoodie</a>
			</div>
			<div class="merch">
                <a href="https://shop.nirvana.com/products/drain-you-crewneck-sweatshirt?_pos=1&_sid=f8d6d8862&_ss=r">Drain You Crewneck Sweatshirt</a>
            </div> 
			<div class="merch">
                <a href="https://shop.nirvana.com/products/abstract-water-crewneck-sweatshirt?_pos=1&_sid=f7540b8df&_ss=r&variant=39439593570393">Abstract Water Crewneck Sweatshirt</a>
            </div> 
			<div class="merch">
                <a href="https://shop.nirvana.com/products/drain-you-zip-hoodie?_pos=1&_sid=00edbaaba&_ss=r">Drain You Zip Hoodie</a>
            </div> 
			<div class="merch">
                <a href="https://shop.nirvana.com/products/dim-light-portrait-tee?_pos=1&_sid=e8fae3711&_ss=r">Dim Light Portrait Tee</a>
            </div> 
			<div class="merch">
				<a href="https://shop.nirvana.com/products/so-happy-tee?_pos=1&_sid=6404a9383&_ss=r">I'm So Happy Smiley Tee</a>
            </div> 
			<div class="merch">
                <a href="https://shop.nirvana.com/products/live-at-reading-black-tee?_pos=1&_sid=8292b576e&_ss=r">Live at Reading Black Tee</a>
            </div> 
			<div class="merch">
                <a href="https://shop.nirvana.com/products/sliver-white-tee?_pos=1&_sid=0db5b9cdf&_ss=r">Sliver Tee - White</a>
            </div> 

		</div>
	</div>
</div>

<style>
	.readable-area {
		display: flex;
		flex-direction: column;
		backdrop-filter: blur(110px);
	}

	.header {
		width: 100vw;
		background-color: black;
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}

	.brandlogo {
		max-width: 200px;
		flex: 1;
		margin-top: 2rem;
	}

	.header h1 {
		margin-bottom: 1rem;
	}

	.content {
		display: flex;
		flex-direction: column;
		justify-content: space-evenly;
	}

	.merchlist {
		padding: 1em;
		display: flex;
		flex-direction: row;
        flex-wrap: wrap;
	}

	.merch {
        margin: 1rem;
		display: flex;
		align-items: flex-end;
		justify-content: center;
        text-align: bottom;
        font-family: Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
		border: 5px #000000 solid;
		border-radius: 15px;
		width: 320px;
	}

	.merch:nth-child(1) {
		width:320px;
		height:352px;
		background-image: url('https://cdn.shopify.com/s/files/1/2081/4611/products/NIRGRITHOODIE.png?v=1632378406');
		background-size: 100%;
		background-repeat:no-repeat;
		transition: 0.5s;
	}

	.merch:nth-child(1):hover {
		background-image: url('https://cdn.shopify.com/s/files/1/2081/4611/products/NIRHOODIE2.png?v=1632378406');
		transform: scale(1.1)
	}

	.merch:nth-child(2) {
		width:320px;
		height:352px;
		background-image: url('https://cdn.shopify.com/s/files/1/2081/4611/products/NIRDRAIN3.png?v=1632378113');
		background-size: 100%;
		background-repeat:no-repeat;
		transition: 0.5s;
	}

	.merch:nth-child(2):hover {
		background-image: url('https://cdn.shopify.com/s/files/1/2081/4611/products/NIRDRAIN1.png?v=1632378113');
		transform: scale(1.1)
	}

	.merch:nth-child(3) {
		width:320px;
		height:352px;
		background-image: url('https://cdn.shopify.com/s/files/1/2081/4611/products/NIRBLUESWEATSHIRT.png?v=1632377629');
		background-size: 100%;
		background-repeat:no-repeat;
		transition: 0.5s;
	}

	.merch:nth-child(3):hover {
		background-image: url('https://cdn.shopify.com/s/files/1/2081/4611/products/NIRSWEATSHIRT2.png?v=1632377629');
		transform: scale(1.1)
	}

	.merch:nth-child(4) {
		width:320px;
		height:352px;
		background-image: url('https://cdn.shopify.com/s/files/1/2081/4611/products/NIRZIP.png?v=1632378251');
		background-size: 100%;
		background-repeat:no-repeat;
		transition: 0.5s;
	}

	.merch:nth-child(4):hover {
		background-image: url('https://cdn.shopify.com/s/files/1/2081/4611/products/NIRZIP3.png?v=1632378251');
		transform: scale(1.1)
	}

	.merch:nth-child(5) {
		width:320px;
		height:352px;
		background-image: url('https://cdn.shopify.com/s/files/1/2081/4611/products/NIRZIP.png?v=1632378251');
		background-size: 100%;
		background-repeat:no-repeat;
		transition: 0.5s;
	}

	.merch:nth-child(5):hover {
		background-image: url('https://cdn.shopify.com/s/files/1/2081/4611/products/NIRZIP3.png?v=1632378251');
		transform: scale(1.1)
	}

	.merch:nth-child(6) {
		width:320px;
		height:352px;
		background-image: url('https://cdn.shopify.com/s/files/1/2081/4611/products/NIRHAPPYTEE.png?v=1613596878');
		background-size: 100%;
		background-repeat:no-repeat;
		transition: 0.5s;
	}

	.merch:nth-child(6):hover {
		background-image: url('https://cdn.shopify.com/s/files/1/2081/4611/products/NIRHAPPYBACKTWW.png?v=1613597529');
		transform: scale(1.1)
	}

	.merch:nth-child(7) {
		width:320px;
		height:352px;
		background-image: url('https://cdn.shopify.com/s/files/1/2081/4611/products/NIRliveatreadingtee.png?v=1596652330');
		background-size: 100%;
		background-repeat:no-repeat;
		transition: 0.5s;
	}

	.merch:nth-child(7):hover {
		background-image: url('https://cdn.shopify.com/s/files/1/2081/4611/products/NIRliveatreadingteefront.png?v=1596652330');
		transform: scale(1.1)
	}

	.merch:nth-child(8) {
		width:320px;
		height:352px;
		background-image: url('https://cdn.shopify.com/s/files/1/2081/4611/products/NIRSLIVERWHITETEE.png?v=1601004158');
		background-size: 100%;
		background-repeat:no-repeat;
		transition: 0.5s;
	}

	.merch:nth-child(8):hover {
		background-image: url('https://cdn.shopify.com/s/files/1/2081/4611/products/NIRsliverwhitefront.png?v=1601004158');
		transform: scale(1.1)
	}
</style>
