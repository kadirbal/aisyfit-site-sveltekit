<script lang="ts">
	import * as m from '$lib/paraglide/messages';

	const steps = [
		{ title: m.hiw_step_1_title, desc: m.hiw_step_1_desc },
		{ title: m.hiw_step_2_title, desc: m.hiw_step_2_desc },
		{ title: m.hiw_step_3_title, desc: m.hiw_step_3_desc },
		{ title: m.hiw_step_4_title, desc: m.hiw_step_4_desc }
	];
</script>

<section id="how-it-works" class="bg-neutral-900/30 py-24">
	<div class="container mx-auto px-6">
		<div class="mb-16 text-center">
			<h2 class="mb-4 text-3xl font-bold md:text-5xl">{m.nav_how_it_works()}</h2>
			<div class="mx-auto h-1 w-24 rounded-full bg-primary"></div>
		</div>

		<div class="grid grid-cols-1 gap-8 md:grid-cols-4">
			{#each steps as step, i}
				<div
					class="group relative rounded-2xl border border-white/5 bg-neutral-950 p-6 transition-colors hover:border-primary/50"
				>
					<div
						class="absolute -top-6 left-1/2 z-10 flex h-12 w-12 -translate-x-1/2 items-center justify-center rounded-full border border-primary bg-neutral-900 text-xl font-bold text-primary transition-transform group-hover:scale-110"
					>
						{i + 1}
					</div>
					<div class="pt-8 text-center">
						<h3 class="mb-3 text-xl font-bold">{step.title()}</h3>
						<p class="text-sm leading-relaxed text-gray-400">{step.desc()}</p>
					</div>
				</div>
			{/each}
		</div>
	</div>
</section>
