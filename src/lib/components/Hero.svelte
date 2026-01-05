<script lang="ts">
	import * as m from '$lib/paraglide/messages';
	import DownloadButtons from './DownloadButtons.svelte';
</script>

<section class="relative flex min-h-screen items-center justify-center overflow-hidden pt-20">
	<!-- Background Elements -->
	<div
		class="pointer-events-none absolute top-0 left-1/2 h-[500px] w-[800px] -translate-x-1/2 rounded-full bg-primary/20 blur-[120px]"
	></div>

	<div class="relative z-10 container mx-auto flex flex-col items-center gap-12 px-6 md:flex-row">
		<!-- Text Content -->
		<div class="flex-1 space-y-8 text-center md:text-left">
			<h1 class="text-5xl leading-tight font-bold whitespace-pre-line md:text-7xl">
				{m.hero_title()}
			</h1>
			<p class="mx-auto max-w-lg text-xl text-gray-400 md:mx-0">
				{m.hero_subtitle()}
			</p>

			<div class="flex justify-center md:justify-start">
				<DownloadButtons alignment="left" />
			</div>

			<div
				class="flex items-center justify-center gap-8 pt-8 text-sm text-gray-500 md:justify-start"
			>
				<div class="flex items-center gap-2">
					<div class="h-2 w-2 rounded-full bg-primary"></div>
					<span>{m.hero_badge_ai()}</span>
				</div>
				<div class="flex items-center gap-2">
					<div class="h-2 w-2 rounded-full bg-primary"></div>
					<span>{m.hero_badge_realtime()}</span>
				</div>
			</div>
		</div>

		<!-- Hero Image -->
		<div class="relative flex-1">
			<div
				class="relative z-10 transform transition-all duration-500 hover:rotate-0 md:rotate-[-5deg]"
			>
				<div class="absolute inset-0 -z-10 rounded-[3rem] bg-primary/20 blur-2xl"></div>
				<img
					src="/images/screenshot-dashboard.png"
					alt="AisyFit Dashboard"
					class="mx-auto w-[300px] rounded-[2.5rem] border-8 border-neutral-900 shadow-2xl"
				/>
			</div>

			<!-- Floating Elements (Optional decoration) -->
			<div
				class="absolute -top-10 -right-10 hidden h-24 w-24 animate-bounce rounded-2xl border border-white/10 bg-neutral-800/80 p-4 backdrop-blur-md md:block"
			>
				<div class="text-2xl font-bold text-primary">540</div>
				<div class="text-xs text-gray-400">Calories Burned</div>
			</div>
		</div>
	</div>
</section>
