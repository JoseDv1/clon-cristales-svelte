<script>
	import Button from './Button.svelte';
</script>

<section id="home">
	<main>
		<img src="/images/cristales-banner.webp" alt="CrisTales" />
		<h1>Available Now</h1>
		<div>
			<Button --text-color="#fff">Stay Updated</Button>
			<Button src="#buy-now" --text-color="#fff">Buy Now</Button>
		</div>
	</main>

	<!-- The video -->
	<video autoplay muted loop>
		<source
			src="https://modusgames.com/cris-tales/wp-content/uploads/sites/2/2021/07/Ct-Launch-Trailer-optimized.mp4"
			type="video/mp4"
		/>
	</video>

	<img src="images/ESRB.png" alt="Teen ESRB" />
	<footer>
		<ul>
			<li><a href="#a"><i class="bx bxl-facebook-square" /></a></li>
			<li><a href="#a"><i class="bx bxl-twitter" /></a></li>
			<li><a href="#a"><i class="bx bxl-youtube" /></a></li>
			<li><a href="#a"><i class="bx bxl-instagram" /></a></li>
			<li><a href="#a"><i class="bx bxl-discord" /></a></li>
			<li><a href="#a"><i class="bx bxs-envelope" /></a></li>
		</ul>
	</footer>
</section>

<style>
	section {
		position: relative;
		width: 100%;
		height: 100dvh;
		font-size: 60px;
		display: grid;
		place-items: center;
	}

	h1 {
		font-size: 60px;
		text-shadow: 0 0 5px #000000;
	}

	/* Cristales Img */
	section main img {
		width: 520px;
		margin-bottom: -40px;
	}

	/* Middle container */
	main {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
	}

	main div {
		display: flex;
		gap: 16px;
	}

	/* ESRB Img */
	section > img {
		width: 190px;
		height: auto;
		position: absolute;
		bottom: 0;
		left: 0;
		margin: 2rem 1rem;
	}

	/* Bg video */
	section video {
		width: 100%;
		height: 100%;
		object-fit: cover;
		position: absolute;
		top: 0;
		z-index: -1;
	}

	/* Footer */
	footer {
		position: absolute;
		bottom: 0;
		right: -2rem;
		padding: 0 4rem 0 2rem;
		height: 50px;
		background: #135a55;
		box-shadow: -0.5rem -0.25rem 0px 0.5rem rgba(0, 0, 0, 0.6);
		display: grid;
		place-items: center;
		transform: skewX(-30deg);
	}

	footer::before {
		background: #135a55;
		bottom: 0;
		box-shadow: -0.5rem -0.25rem 0px 0px rgba(0, 0, 0, 0.6);
		content: '';
		display: block;
		height: 1rem;
		position: absolute;
		right: 100%;
		width: 100dvw;
	}

	footer ul,
	footer li {
		height: 100%;
	}

	footer ul {
		list-style: none;
		display: flex;
		width: 100%;
		gap: 1rem;
	}

	footer li {
		border-right: 1px solid #01bfaf;
		padding: 0 1rem 0 0;
	}

	footer li:last-child {
		border-right: none;
		padding-right: 0;
	}

	footer a {
		color: #fff;
		width: 100%;
		height: 100%;
		display: grid;
		place-items: center;
	}

	footer i {
		color: #01bfaf;
		transform: skewX(30deg);
		font-size: 2rem;
	}

	@media (max-width: 768px) {
	}
</style>
