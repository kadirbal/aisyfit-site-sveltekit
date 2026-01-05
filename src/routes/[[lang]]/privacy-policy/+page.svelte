<script lang="ts">
	import PrivacyPolicyDisplay from '$lib/components/legal/PrivacyPolicyDisplay.svelte';
	import { getLocale } from '$lib/paraglide/runtime';

	let title = $derived(
		getLocale() === 'tr' ? 'Gizlilik Politikası | AisyFit' : 'Privacy Policy | AisyFit'
	);
	let description = $derived(
		getLocale() === 'tr'
			? 'AisyFit Gizlilik Politikası. Verilerinizi nasıl koruduğumuzu öğrenin.'
			: 'Privacy Policy for AisyFit. Learn how we protect your data.'
	);
</script>

<svelte:head>
	<title>{title}</title>
	<meta name="description" content={description} />
</svelte:head>

<div class="relative min-h-screen bg-black pt-24 pb-12 text-white">
	<div
		class="absolute top-0 -left-40 h-[500px] w-[500px] rounded-full bg-primary/5 blur-[100px]"
	></div>
	<div class="relative container mx-auto px-6">
		<PrivacyPolicyDisplay />
	</div>
</div>
