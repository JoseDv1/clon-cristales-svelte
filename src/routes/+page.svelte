<script>
	import DarkBlueSection from '$lib/components/DarkBlueSection.svelte';
	import Navbar from '$lib/components/Navbar.svelte';
	import VideoSection from '$lib/components/VideoSection.svelte';
	import GreenSection from '$lib/components/GreenSection.svelte';
	import NewsSection from '$lib/components/NewsSection.svelte';
	import GalerySection from '$lib/components/GalerySection.svelte';
	import CommunitySection from '$lib/components/CommunitySection.svelte';
	import Footer from '../lib/components/Footer.svelte';
</script>

<section>
	<Navbar />

	<div>
		<VideoSection />
	</div>
	<div>
		<DarkBlueSection />
	</div>
	<div>
		<GreenSection />
	</div>
	<div>
		<NewsSection />
	</div>
	<div>
		<GalerySection />
	</div>
	<div>
		<CommunitySection />
	</div>

	<Footer />
</section>

<style>
	section {
		scroll-snap-type: y mandatory;
		overflow-y: scroll;
		overflow-x: hidden;
		height: 100vh;
	}

	div {
		scroll-snap-align: center;
	}
</style>
