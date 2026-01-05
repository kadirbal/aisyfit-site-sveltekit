<script>
	import Features from '$lib/components/Features.svelte';
	import Footer from '$lib/components/Footer.svelte';
	import Hero from '$lib/components/Hero.svelte';
	import HowItWorks from '$lib/components/HowItWorks.svelte';
	import Personalization from '$lib/components/Personalization.svelte';
</script>

<svelte:head>
	<title>AisyFit - AI Fitness Coach</title>
</svelte:head>

<main class="min-h-screen bg-black text-white selection:bg-primary selection:text-black">
	<Hero />
	<div id="how-it-works">
		<HowItWorks />
	</div>
	<div id="personalization">
		<Personalization />
	</div>
	<Features />
	<Footer />
</main>
