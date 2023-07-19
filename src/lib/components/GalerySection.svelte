<script>
	import GreenCard from './GreenCard.svelte';
</script>

<section id="media">
	<h1>Media</h1>

	<GreenCard>
		<section class="galery">
			<div><img src="/images/galery/galery-1.jpg" alt="Galery" /></div>
			<div><img src="/images/galery/galery-2.jpg" alt="Galery" /></div>
			<div><img src="/images/galery/galery-3.jpg" alt="Galery" /></div>
			<div><img src="/images/galery/galery-4.jpg" alt="Galery" /></div>
			<div><img src="/images/galery/galery-5.jpg" alt="Galery" /></div>
			<div><img src="/images/galery/galery-6.jpg" alt="Galery" /></div>
		</section>
	</GreenCard>
</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		width: 100%;
		height: 100%;
		padding: 3rem;
	}

	.galery {
		display: grid;
		grid-template-columns: repeat(auto-fit, minmax(400px, 1fr));
		gap: 3rem;
	}

	.galery div {
		width: 100%;
		height: 100%;
		overflow: hidden;
	}

	.galery div img {
		width: 100%;
		height: 100%;
		object-fit: cover;
		transition: transform 0.3s ease-in-out;
	}

	.galery div img:hover {
		transform: scale(1.2);
	}
</style>
