<script lang="ts">
	import * as m from '$lib/paraglide/messages';

	// We need to construct the array reactively or call functions in the template
	// But easier to just instantiate inside the template loops or reactive statement
	// Let's make it a derived variable

	const features = [
		{
			title_fn: m.feature_1_title,
			desc_fn: m.feature_1_desc,
			image: '/images/screenshot-workout.png',
			align: 'left'
		},
		{
			title_fn: m.feature_2_title,
			desc_fn: m.feature_2_desc,
			image: '/images/screenshot-diet.png',
			align: 'right'
		},
		{
			title_fn: m.feature_3_title,
			desc_fn: m.feature_3_desc,
			image: '/images/screenshot-progress.png',
			align: 'left'
		}
	];
</script>

<section class="relative py-24">
	<div class="container mx-auto px-6">
		<div class="mb-20 text-center">
			<h2 class="mb-4 text-3xl font-bold whitespace-pre-line md:text-5xl">{m.features_title()}</h2>
			<p class="mx-auto max-w-2xl text-gray-400">{m.features_subtitle()}</p>
		</div>

		<div class="space-y-32">
			{#each features as feature, i}
				<div
					class="flex flex-col items-center gap-12 md:flex-row md:gap-24 {feature.align === 'right'
						? 'md:flex-row-reverse'
						: ''}"
				>
					<!-- Image Side -->
					<div class="group relative flex-1">
						<div
							class="absolute inset-0 bg-gradient-to-tr from-primary/20 to-transparent opacity-0 blur-3xl transition-opacity duration-500 group-hover:opacity-100"
						></div>
						<img
							src={feature.image}
							alt={feature.title_fn()}
							class="relative z-10 mx-auto w-[280px] transform rounded-[2.5rem] border-8 border-neutral-800 shadow-2xl transition-transform duration-500 group-hover:scale-105 group-hover:-rotate-2"
						/>
					</div>

					<!-- Content Side -->
					<div class="flex-1 text-center md:text-left">
						<div
							class="mb-6 inline-block rounded-full border border-white/10 bg-neutral-800 px-4 py-1 text-sm font-medium text-primary"
						>
							0{i + 1}
						</div>
						<h3 class="mb-6 text-3xl font-bold md:text-4xl">{feature.title_fn()}</h3>
						<p class="mb-8 text-lg leading-relaxed text-gray-400">
							{feature.desc_fn()}
						</p>
						<button
							class="mx-auto flex items-center gap-2 font-medium text-white transition-colors hover:text-primary md:mx-0"
						>
							{m.features_learn_more()}
							<svg
								xmlns="http://www.w3.org/2000/svg"
								fill="none"
								viewBox="0 0 24 24"
								stroke-width="1.5"
								stroke="currentColor"
								class="h-5 w-5"
							>
								<path
									stroke-linecap="round"
									stroke-linejoin="round"
									d="M13.5 4.5 21 12m0 0-7.5 7.5M21 12H3"
								/>
							</svg>
						</button>
					</div>
				</div>
			{/each}
		</div>
	</div>
</section>
