<script>
	import BlueCard from './BlueCard.svelte';
	import GreenCard from './GreenCard.svelte';
	import PinkCard from './PinkCard.svelte';
</script>

<section id="news">
	<div>
		<h1>News</h1>
		<PinkCard>
			<div>
				<img src="images/news/adri-joins.jpg" alt="Adri _Joins" />
				<h2>Cris Tales Content Update, Patch Notes, and Holiday Sales!</h2>

				<small>December 16, 2021</small>
				<p>
					Today we unleash a flurry of free content for Cris Tales, including a brand-new character,
					dungeon, cutscene and much more! Beyond these additions, this free update adds new story
					content such as a new ending and all-new cutscene. Holiday shoppers can also enjoy steep
					discounts this month on Steam, Nintendo Switch and Xbox. Keep reading...
				</p>
			</div>
			<a href=""> Continue Reading </a>
		</PinkCard>
		<BlueCard>
			<div>
				<img src="images/news/latestnews.jpg" alt="Latest news" />
				<h2>Keep Up with the Latest Patch Notes for Cris Tales Here</h2>

				<small>August 30, 2021</small>
				<p>
					We have been listening to and collecting feedback from our community, and we have our
					first patch available for Cris Tales. We will update this blog with additional patch notes
					as they come available. If you’d like to give additional feedback, you can find us on
					Twitter or join our Discord. Keep reading to see detailed patch notes...
				</p>
			</div>
			<a href=""> Continue Reading </a>
		</BlueCard>
		<GreenCard>
			<div>
				<img src="images/news/cristalespreviewround.jpg" alt=" Preview" />
				<h2>Cris Tales Preview Round-Up</h2>

				<small>June 16, 2021</small>
				<p>
					Cris Tales launches next month, and in preparation for the game’s release, we gave press a
					sneak peek at some extended gameplay. The preview footage showed off the first 3 kingdoms
					players will explore. Check out the list below for some of the coverage! WCCFTech: Cris
					Tales Preview - A Deep Dive Into the Timestream:...
				</p>
			</div>
			<a href=""> Continue Reading </a>
		</GreenCard>
	</div>
</section>

<style>
	section {
		display: flex;
		flex-wrap: wrap;
		justify-content: center;
		gap: 2rem;
		width: 100dvw;
		padding: 2rem;
	}

	section > div {
		display: flex;
		flex-wrap: wrap;
		gap: 2rem;
		width: 100%;
	}

	section div > * {
		width: 100%;
	}

	section div div {
		position: relative;
		display: flex;
		flex-direction: column;
		gap: 0.5rem;
	}

	section div h2 {
		color: #e95095;
	}

	small,
	p {
		font-family: liberation-sans, sans-serif;
	}

	a {
		position: absolute;
		bottom: 0;
		right: 50%;
		transform: translateX(50%);
		background-color: #e95095;
		padding: 4px 20px;
		font-family: liberation-sans, sans-serif;
		font-size: 16px;
		border-radius: 0.5rem 0.5rem 0 0;
		transition: all 0.2s ease-in-out;
		display: grid;
		place-items: center;
		height: 30px;
	}

	a:hover {
		color: #7049ba;
		height: 40px;
	}

	:global(section#news section.card) {
		width: calc(33% - 2rem);
	}
</style>
