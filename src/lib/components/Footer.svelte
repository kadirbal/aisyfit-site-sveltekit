<script lang="ts">
	import * as m from '$lib/paraglide/messages';
</script>

<footer class="mt-20 border-t border-white/5 bg-neutral-900/50 py-12">
	<div class="container mx-auto px-6">
		<div class="flex flex-col items-center justify-between gap-8 md:flex-row">
			<div class="text-2xl font-bold tracking-tighter">
				AISY<span class="text-primary">FIT</span>
			</div>

			<div class="flex gap-8 text-sm text-gray-400">
				<a href="/" class="transition-colors hover:text-primary">{m.footer_privacy()}</a>
				<a href="/" class="transition-colors hover:text-primary">{m.footer_terms()}</a>
				<a href="/" class="transition-colors hover:text-primary">{m.footer_contact()}</a>
			</div>

			<div class="text-sm text-gray-600">
				{m.footer_rights()}
			</div>
		</div>
	</div>
</footer>
