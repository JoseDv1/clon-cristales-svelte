<nav>
	<img src="/images/cristales-logo.png" alt="Cristales" />
	<ul>
		<li><a href="#home">Home</a></li>
		<li><a href="#about">About</a></li>
		<li><a href="#news">News</a></li>
		<li><a href="#media">Media</a></li>
		<li><a href="#community">Community</a></li>
		<li><a href="#buy-now">Buy Now</a></li>
		<li><a href="https://store.maximumgames.com/">Store</a></li>
		<li><a href="https://modusgames.com/">All Modus Games</a></li>
	</ul>
</nav>

<style>
	nav {
		position: fixed;
		width: 100%;

		display: flex;
		justify-content: space-between;
		align-items: center;

		padding: 0 40px;
		background: #02393c91;
		border-bottom: #00756b dashed 4px;
		font-size: 22px;
		z-index: 1;
	}

	nav ul {
		list-style: none;
		display: flex;
	}

	nav ul li a {
		padding: 0 20px;
	}

	nav ul li a:hover {
		color: #01bfaf;
	}

	nav img {
		width: 210px;
	}

	@media (max-width: 768px) {
		nav ul {
			display: none;
		}
	}
</style>
