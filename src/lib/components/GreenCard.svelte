<section class="card">
	<div>
		<slot />
	</div>
</section>

<style>
	section {
		position: relative;
		background: #00404499;
		border: 4px solid #416769;
		color: #4bc1b7;
	}

	div {
		position: relative;
		width: 100%;
		height: 100%;
		padding: 40px 40px 50px;
	}

	::before,
	::after {
		content: '';
		background-image: url('/images/corners/green-corner.png');
		background-size: 100% 100%;
		background-repeat: no-repeat;
		position: absolute;
		width: 80px;
		aspect-ratio: 1/1;
	}

	section::before {
		top: 0;
		left: 0;
	}

	section::after {
		top: 0;
		right: 0;
		transform: rotate(90deg);
	}

	div::after {
		bottom: 0;
		right: 0;
		transform: rotate(180deg);
	}

	div::before {
		bottom: 0;
		left: 0;
		transform: rotate(270deg);
	}
</style>
