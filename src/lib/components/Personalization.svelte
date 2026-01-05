<script lang="ts">
	import * as m from '$lib/paraglide/messages';
</script>

<section id="personalization" class="relative overflow-hidden py-24">
	<!-- Decorative background -->
	<div
		class="absolute top-0 right-0 h-96 w-96 translate-x-1/2 -translate-y-1/2 rounded-full bg-primary/5 blur-3xl"
	></div>

	<div class="relative z-10 container mx-auto px-6">
		<div class="flex flex-col items-center gap-16 md:flex-row">
			<div class="flex-1">
				<h2 class="mb-6 text-3xl font-bold md:text-5xl">{m.pers_title()}</h2>
				<p class="mb-8 text-xl text-gray-300">{m.pers_subtitle()}</p>

				<div class="space-y-6">
					<!-- Card 1 -->
					<div class="flex items-start gap-4 rounded-xl border border-white/5 bg-white/5 p-4">
						<div class="rounded-lg bg-primary/20 p-3 text-primary">
							<svg
								xmlns="http://www.w3.org/2000/svg"
								class="h-6 w-6"
								fill="none"
								viewBox="0 0 24 24"
								stroke="currentColor"
							>
								<path
									stroke-linecap="round"
									stroke-linejoin="round"
									stroke-width="2"
									d="M13 10V3L4 14h7v7l9-11h-7z"
								/>
							</svg>
						</div>
						<div>
							<h3 class="text-lg font-bold">{m.pers_card_goals()}</h3>
							<p class="text-sm text-gray-400">{m.pers_card_goals_desc()}</p>
						</div>
					</div>

					<!-- Card 2 -->
					<div class="flex items-start gap-4 rounded-xl border border-white/5 bg-white/5 p-4">
						<div class="rounded-lg bg-primary/20 p-3 text-primary">
							<svg
								xmlns="http://www.w3.org/2000/svg"
								class="h-6 w-6"
								fill="none"
								viewBox="0 0 24 24"
								stroke="currentColor"
							>
								<path
									stroke-linecap="round"
									stroke-linejoin="round"
									stroke-width="2"
									d="M3 6l3 1m0 0l-3 9a5.002 5.002 0 006.001 0M6 7l3 9M6 7l6-2m6 2l3-1m-3 1l-3 9a5.002 5.002 0 006.001 0M18 7l3 9m-3-9l-6-2m0-2v2m0 16V5m0 16H9m3 0h3"
								/>
							</svg>
						</div>
						<div>
							<h3 class="text-lg font-bold">{m.pers_card_diet()}</h3>
							<p class="text-sm text-gray-400">{m.pers_card_diet_desc()}</p>
						</div>
					</div>

					<!-- Card 3 -->
					<div class="flex items-start gap-4 rounded-xl border border-white/5 bg-white/5 p-4">
						<div class="rounded-lg bg-primary/20 p-3 text-primary">
							<svg
								xmlns="http://www.w3.org/2000/svg"
								class="h-6 w-6"
								fill="none"
								viewBox="0 0 24 24"
								stroke="currentColor"
							>
								<path
									stroke-linecap="round"
									stroke-linejoin="round"
									stroke-width="2"
									d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z"
								/>
							</svg>
						</div>
						<div>
							<h3 class="text-lg font-bold">{m.pers_card_injuries()}</h3>
							<p class="text-sm text-gray-400">{m.pers_card_injuries_desc()}</p>
						</div>
					</div>
				</div>
			</div>

			<!-- Feature Image -->
			<div class="relative flex-1">
				<div
					class="relative z-10 transform transition-all duration-500 hover:rotate-0 md:rotate-[2deg]"
				>
					<div class="absolute inset-0 -z-10 rounded-[3rem] bg-primary/20 blur-2xl"></div>
					<img
						src="/images/screenshot-settings.png"
						alt="Profile Settings"
						class="mx-auto w-[300px] rounded-[2.5rem] border-8 border-neutral-900 shadow-2xl"
					/>
				</div>
			</div>
		</div>
	</div>
</section>
