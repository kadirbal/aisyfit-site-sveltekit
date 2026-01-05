<script lang="ts">
	import { page } from '$app/stores';
	import * as m from '$lib/paraglide/messages';
	import { getLocale, locales } from '$lib/paraglide/runtime';

	const names = {
		en: 'EN',
		tr: 'TR'
	};

	function switchTo(locale: string) {
		const path = $page.url.pathname;
		const current = getLocale();
		let newPath = path;

		if (current === 'en' && locale === 'tr') {
			// If current is en (root /), adding /tr prefix
			newPath = '/tr' + (path === '/' ? '' : path);
		} else if (current === 'tr' && locale === 'en') {
			// If current is tr, remove /tr prefix
			newPath = path.replace(/^\/tr/, '') || '/';
		}

		return newPath;
	}

	function scrollToSection(id: string) {
		const element = document.getElementById(id);
		if (element) {
			element.scrollIntoView({ behavior: 'smooth' });
		}
	}
</script>

<header
	class="fixed top-0 left-0 z-50 w-full border-b border-white/5 bg-neutral-900/10 backdrop-blur-md transition-all duration-300"
>
	<div class="container mx-auto flex h-20 items-center justify-between px-6">
		<!-- Logo -->
		<a href="/" class="text-2xl font-bold tracking-tighter transition-colors hover:text-primary">
			AISY<span class="text-primary">FIT</span>
		</a>

		<!-- Desktop Nav -->
		<nav class="hidden items-center gap-8 md:flex">
			<button
				onclick={() => scrollToSection('how-it-works')}
				class="text-sm font-medium text-gray-300 transition-colors hover:text-primary"
			>
				{m.nav_how_it_works()}
			</button>
			<button
				onclick={() => scrollToSection('personalization')}
				class="text-sm font-medium text-gray-300 transition-colors hover:text-primary"
			>
				{m.nav_personalization()}
			</button>
		</nav>

		<!-- Language Switcher & CTA -->
		<div class="flex items-center gap-4">
			<div class="flex items-center rounded-full border border-white/5 bg-black/20 p-1">
				{#each locales as locale}
					<a
						href={switchTo(locale)}
						class="rounded-full px-3 py-1 text-xs font-bold transition-all {getLocale() === locale
							? 'bg-primary text-black shadow-lg shadow-primary/20'
							: 'text-gray-400 hover:text-white'}"
						data-sveltekit-reload
					>
						{names[locale]}
					</a>
				{/each}
			</div>

			<button
				class="hidden rounded-full border border-white/10 bg-white/5 px-6 py-2 text-sm font-bold transition-all hover:border-primary hover:bg-primary hover:text-black md:block"
			>
				{m.hero_cta_start()}
			</button>
		</div>
	</div>
</header>
