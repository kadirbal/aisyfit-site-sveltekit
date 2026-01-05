<script lang="ts">
	import * as m from '$lib/paraglide/messages';
	import DownloadButtons from './DownloadButtons.svelte';
</script>

<section class="relative overflow-hidden py-24">
	<!-- Glow Effect -->
	<div
		class="pointer-events-none absolute bottom-0 left-1/2 h-[400px] w-[600px] -translate-x-1/2 rounded-full bg-primary/10 blur-[100px]"
	></div>

	<div class="relative z-10 container mx-auto px-6 text-center">
		<h2 class="mb-6 text-4xl font-bold tracking-tight md:text-6xl">{m.download_title()}</h2>
		<p class="mx-auto mb-12 max-w-2xl text-xl text-gray-400">{m.download_subtitle()}</p>

		<DownloadButtons alignment="center" />
	</div>
</section>
