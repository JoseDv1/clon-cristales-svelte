<script>
	import BlueCard from './BlueCard.svelte';
	import GreenCard from './GreenCard.svelte';
	import PinkCard from './PinkCard.svelte';
</script>

<section id="community">
	<BlueCard>
		<article class="involved">
			<h1>Get Involved</h1>
			<div>
				<a href="http://twitter.com/Modus_Games"><i class="bx bxl-twitter" />Follow Us On Twitter</a
				>
				<a href="http://discord.gg/modus"> <i class="bx bxl-discord" />Join Our Discord</a>
				<a href="http://www.facebook.com/ModusGames/">
					<i class="bx bxl-facebook-square" />
					Like Us On Facebook</a
				>
			</div>
		</article>
	</BlueCard>
	<GreenCard
		><article class="support">
			<h1>Support Cris Tales</h1>
			<div>
				<a href="#buy-now"><i class="bx bx-cart-alt" />Buy Cris Tales</a>
				<a
					href="https://store.steampowered.com/app/1079830/Cris_Tales/?&utm_source=modus&utm_medium=website"
					><i class="bx bxl-steam" />Wish List On Steam</a
				>
			</div>
		</article>
	</GreenCard>
	<PinkCard>
		<article class="updated">
			<h1>Stay Updated</h1>
			<div>
				<a href="#community"><i class="bx bxs-bell" />Sign Up For Emails</a>
			</div>
		</article>
	</PinkCard>
</section>

<style>
	section {
		display: flex;
		width: 100%;
		height: 100%;
		padding: 3rem;
		gap: 2rem;
	}

	:global(section#community > *) {
		flex: 1;
	}

	article {
		display: flex;
		flex-direction: column;
		align-items: center;
		height: 100%;
	}

	div {
		display: flex;
		justify-content: center;
		align-items: center;
		gap: 1rem;
		flex-wrap: wrap-reverse;
	}

	a {
		display: flex;
		justify-content: center;
		align-items: center;
		padding: 1rem;
		border-radius: 0.5rem;
		font-family: liberation-sans, sans-serif;
		gap: 0.5rem;
		width: 220px;
		transition: background-color 0.2s ease-in-out;
	}

	.involved a:first-child {
		background-color: #1da1f2;
	}

	.involved a:nth-child(2) {
		background-color: #2b54a5;
	}

	.involved a:last-child {
		background-color: #3b5998;
	}

	.involved a:first-child:hover {
		background-color: #05a0dc;
	}

	.involved a:nth-child(2):hover {
		background-color: #264a90;
	}

	.involved a:last-child:hover {
		background-color: #344d84;
	}

	i {
		font-size: 4rem;
	}

	.support a:first-child {
		background: #15655e;
	}

	.support a:first-child:hover {
		background: #125650;
	}

	.support a:last-child {
		background: #01bfaf;
	}

	.support a:last-child:hover {
		background: #039c8f;
	}

	.updated a {
		background: #8224a0;
	}

	.updated a:hover {
		background: #6a1d8a;
	}
</style>
