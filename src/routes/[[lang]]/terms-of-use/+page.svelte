<script lang="ts">
	import TermsOfUseDisplay from '$lib/components/legal/TermsOfUseDisplay.svelte';
	import { getLocale } from '$lib/paraglide/runtime';

	let title = $derived(
		getLocale() === 'tr' ? 'Kullanım Koşulları | AisyFit' : 'Terms of Use | AisyFit'
	);
	let description = $derived(
		getLocale() === 'tr'
			? 'AisyFit Kullanım Koşulları. Hizmetlerimizi kullanırken uymanız gereken kurallar.'
			: 'Terms of Use for AisyFit. Rules and regulations for using our services.'
	);
</script>

<svelte:head>
	<title>{title}</title>
	<meta name="description" content={description} />
</svelte:head>

<div class="relative min-h-screen bg-black pt-24 pb-12 text-white">
	<div
		class="absolute top-0 -right-40 h-[500px] w-[500px] rounded-full bg-primary/5 blur-[100px]"
	></div>
	<div class="relative container mx-auto px-6">
		<TermsOfUseDisplay />
	</div>
</div>
