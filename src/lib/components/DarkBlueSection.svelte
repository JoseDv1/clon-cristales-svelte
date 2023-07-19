<script>
	import { onMount } from 'svelte';
	import BlueCard from './BlueCard.svelte';
	import Button from './Button.svelte';

	let buttons;

	onMount(() => {
		buttons.childNodes[0].style.backgroundColor = '#004044';
	});

	const standardClick = () => {
		buttons.childNodes[0].style.backgroundColor = '#004044';
		buttons.childNodes[2].style.backgroundColor = null;
	};

	const collectorsClick = () => {
		console.log(buttons.childNodes);
		buttons.childNodes[0].style.backgroundColor = null;
		buttons.childNodes[2].style.backgroundColor = '#004044';
	};
</script>

<section id="buy-now">
	<BlueCard>
		<div class="img-card">
			<h1>Award Winning RPG</h1>
			<img src="/images/acolades.png" alt="" />
		</div>
	</BlueCard>
	<BlueCard>
		<div class="form-card">
			<h1>Buy Now</h1>
			<!-- svelte-ignore a11y-click-events-have-key-events -->
			<!-- svelte-ignore a11y-no-noninteractive-element-interactions -->
			<div class="buttons" bind:this={buttons}>
				<!-- svelte-ignore a11y-click-events-have-key-events -->
				<!-- svelte-ignore a11y-no-noninteractive-element-interactions -->
				<p on:click={standardClick}>Standard Edition</p>
				<p on:click={collectorsClick}>Collector's Edition</p>
			</div>
			<form>
				<select>
					<option>Physical</option>
					<option>Digital</option>
				</select>
				<select>
					<option>Select Platform</option>
					<option>PC</option>
					<option>PS4</option>
					<option>PS5</option>
					<option>Nintendo Switch</option>
					<option>Xbox One</option>
					<option>Xbox Series XS</option>
				</select>
				<select>
					<option>Select Region</option>
					<option>North America</option>
					<option>South America</option>
					<option>Europe</option>
					<option>Asia</option>
					<option>Australia</option>
					<option>Africa</option>
				</select>
				<select>
					<option>Select Retailer</option>
					<option>Amazon</option>
					<option>Steam</option>
					<option>Playstation Store</option>
					<option>Xbox Store</option>
					<option>Nintendo Store</option>
				</select>
				<Button --text-color="#fff">Buy Now</Button>
			</form>
		</div>
	</BlueCard>
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

	.img-card,
	.form-card {
		display: flex;
		flex-direction: column;
		align-items: center;
		gap: 1.5rem;
		justify-content: center;
		width: 100%;
	}

	.img-card img {
		width: 100%;
		height: auto;
	}

	.form-card form {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		width: 100%;
		padding: 0 4rem;
	}

	.form-card form select {
		width: 100%;
		height: 3rem;
		margin-bottom: 1rem;
		padding: 0 1rem;
		border-radius: 0.5rem;
		border: none;
	}

	.form-card form select:focus {
		outline: none;
	}

	.buttons {
		display: flex;
		align-items: center;
		justify-content: center;
		width: 100%;
		margin-bottom: 1rem;
		gap: 4rem;
	}

	.buttons p {
		font-family: liberation-sans, sans-serif;
		font-size: 24px;
		display: block;
		padding: 0.5rem 2rem;
		border: 3px solid #416769;
		cursor: pointer;
	}

	:global(.form-card form a) {
		align-self: flex-start;
	}

	:global(section#buy-now > section.card) {
		width: calc(50% - 2rem);
	}
</style>
