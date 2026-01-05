<script>
  import Hero from '$lib/components/Hero.svelte';
  import Features from '$lib/components/Features.svelte';
  import Footer from '$lib/components/Footer.svelte';
</script>

<svelte:head>
  <title>AisyFit - AI Fitness Coach</title>
</svelte:head>

<main class="min-h-screen bg-black text-white selection:bg-primary selection:text-black">
  <Hero />
  <Features />
  <Footer />
</main>
