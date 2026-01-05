<script>
	import Features from '$lib/components/Features.svelte';
	import Footer from '$lib/components/Footer.svelte';
	import Hero from '$lib/components/Hero.svelte';
	import HowItWorks from '$lib/components/HowItWorks.svelte';
	import LanguageSwitcher from '$lib/components/LanguageSwitcher.svelte';
	import Personalization from '$lib/components/Personalization.svelte';
</script>

<svelte:head>
	<title>AisyFit - AI Fitness Coach</title>
</svelte:head>

<main class="min-h-screen bg-black text-white selection:bg-primary selection:text-black">
	<LanguageSwitcher />
	<Hero />
	<HowItWorks />
	<Personalization />
	<Features />
	<Footer />
</main>
