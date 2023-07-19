<script>
	import GreenCard from './GreenCard.svelte';
</script>

<section id="about">
	<GreenCard>
		<div class="video-card">
			<h1>About Cris Tales</h1>
			<iframe
				title="YouTube video player"
				loading="lazy"
				src="https://www.youtube.com/embed/T_pq_Q2dwRQ"
				frameborder="0"
				allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
				allowfullscreen=""
			/>
			<p>
				Cris Tales is a gorgeous, indie love letter to classic JRPGs with a new perspective. Peer
				into the past, act in the present, and watch as your choices dynamically change the future —
				all on one screen as you play! Beautifully hand-drawn 2D animations bring to life a world
				where your choices will change both the present and the future across more than 20 hours of
				gameplay.
			</p>
		</div>
	</GreenCard>
	<GreenCard>
		<div class="features">
			<h1>Key Features</h1>

			<p>
				<strong>A Love Letter to Classic JRPGs</strong> <br /> Inspired by timeless JRPGs like Chrono
				Trigger, Final Fantasy VI, Valkyrie Profile, and modern classics like Bravely Default and Persona
				5, meet and recruit a unique cast of teammates, challenge myriad enemies, and make your way through
				an expansive world.
			</p>
			<p>
				<strong>Experience the Past, Present, and Future Simultaneously</strong> <br /> Peer into and
				learn from the past, decide on actions in the present, and alter the course of the future in
				ways that will reshape the world dynamically depending on the choices you make.
			</p>
			<p>
				<strong>Master Strategic Turn-Based Combat</strong> <br /> Warp your enemies into the past or
				future, synchronize attacks for enhanced group abilities, and master the timing of attack and
				defense to go beyond your party’s limits in combat.
			</p>
			<p>
				<strong>Uncover a Fascinating Story & Characters</strong> <br /> The Empress’ plot to destroy
				the world is complex and layered. Use your wits and recruit powerful allies throughout the world
				to uncover and undo her multi-faceted web and make your way to the True Ending of this enchanting
				tale.
			</p>
			<p>
				<strong>Discover a Beautiful World</strong> <br /> Climb aboard an airship or boat and traverse
				this handcrafted, dark fairytale world. From the shining kingdom of Crystallis to the slums of
				Saint Clarity, discover each unique location and shape its future.
			</p>
		</div>
	</GreenCard>
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

	.features,
	.video-card {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		gap: 1.5rem;
		width: 100%;
	}

	.video-card iframe {
		width: 100%;
		height: 50vh;
	}

	.video-card p {
		width: 100%;
		text-align: center;
	}

	.features p {
		position: relative;
		padding-left: 40px;
	}

	.features p::before {
		background: url('/images/bullet.webp');
		content: '';
		height: 32px;
		width: 32px;
		left: 0;
		position: absolute;
		top: 0;
	}

	.features h1 {
		align-self: flex-start;
	}

	p {
		font-size: 18px;
		font-family: liberation-sans, sans-serif;
		color: #fff;
		line-height: 25px;
	}

	strong {
		font-size: 20px;
		font-family: liberation-sans, sans-serif;
		font-weight: bold;
	}

	:global(section#about > section.card) {
		width: calc(50% - 2rem);
	}
</style>
