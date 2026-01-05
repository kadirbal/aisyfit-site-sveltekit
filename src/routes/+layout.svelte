<script lang="ts">
	import Header from '$lib/components/Header.svelte';
	import '../routes/layout.css';
</script>

<svelte:head>
	<link rel="icon" href="/favicon.png" />
</svelte:head>

<Header />
<slot />
