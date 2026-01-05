<script lang="ts">
	import { page } from '$app/stores';
	import { getLocale, locales } from '$lib/paraglide/runtime';

	// Map locale to display name
	const names = {
		en: 'EN',
		tr: 'TR'
	};

	/**
	 * Helper to switch language by modifying the URL
	 */
	function switchTo(locale: string) {
		const path = $page.url.pathname;
		const current = getLocale();

		let newPath = path;

		// Build URL based on simple path replacement for now
		if (current === 'en' && locale === 'tr') {
			newPath = '/tr' + (path === '/' ? '' : path);
		} else if (current === 'tr' && locale === 'en') {
			newPath = path.replace(/^\/tr/, '') || '/';
		}

		return newPath;
	}
</script>

<div
	class="fixed top-6 right-6 z-50 flex gap-2 rounded-full border border-white/10 bg-neutral-900/80 p-1 backdrop-blur"
>
	{#each locales as locale}
		<a
			href={switchTo(locale)}
			class="rounded-full px-3 py-1 text-sm font-bold transition-colors {getLocale() === locale
				? 'bg-primary text-black'
				: 'text-gray-400 hover:text-white'}"
			data-sveltekit-reload
		>
			{names[locale]}
		</a>
	{/each}
</div>
