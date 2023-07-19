<script>
	import Button from './Button.svelte';
</script>

<section>
	<div class="btns">
		<Button src="https://modusgames.com/support/" --text-color="#fff">Suppport</Button>
		<Button src="/" --text-color="#fff">Press inquires</Button>
	</div>

	<div class="platforms">
		<img src="/images/platforms/switch.webp" alt="Nintendo Switch" />
		<img src="/images/platforms/ps4.png" alt="ps4" />
		<img src="/images/platforms/ps5.png" alt="ps5" />
		<img src="/images/platforms/xboxone.png" alt="Xbox One" />
		<img src="/images/platforms/xboxx.png" alt="Xbox Series X" />
		<img src="/images/platforms/steam.png" alt="Steam" />
		<img src="/images/platforms/stadia.png" alt="Google Stadia" />
		<img src="/images/platforms/epicgames.png" alt="Epic Games" />
		<img src="/images/platforms/gogcom.png" alt="Gog Com" />
	</div>

	<img src="/images/ESRB.png" alt="ESRB" />

	<div class="devs">
		<img src="/images/devs/moduslogo.png" alt="" />
		<img src="/images/devs/dreamlogo.png" alt="" />
		<img src="/images/devs/sycklogo.png" alt="" />
	</div>

	<p>
		© 2021 Dreams Uncorpored LLC. Published by Modus Games™. Modus Games™ and the Modus™ logo are
		trademarks of Modus Games, LLC. All rights reserved. <br />Nintendo Switch is a trademark of
		Nintendo. <br /> All other trademarks or registered trademarks belong to their respective owners.
	</p>
</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		width: 100%;
		height: 100%;
		padding: 3rem;
		gap: 2rem;
	}

	.btns {
		display: flex;
		justify-content: flex-end;
		align-items: center;
		gap: 1rem;
		width: 100%;
	}

	.platforms,
	.devs {
		display: flex;
		justify-content: center;
		align-items: space-around;
		gap: 2rem;
		width: 100%;
	}

	.platforms img,
	.devs img {
		height: 4rem;
	}

	img[alt='ESRB'] {
		width: 15%;
		align-self: center;
	}

	p {
		text-align: center;
		color: #fff;
	}
</style>
