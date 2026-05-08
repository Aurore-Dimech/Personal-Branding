<script lang="ts">
	import './layout.css';
	import favicon from '$lib/assets/logo.svg';
	import Footer from '$lib/components/layouts/Footer.svelte';
	import Header from '$lib/components/layouts/Header.svelte';

	const { children } = $props();
</script>

<svelte:head><link rel="icon" href={favicon} /></svelte:head>

<div class="flex h-screen w-screen flex-col font-montserrat" id="top">
	<Header />

	<main
		class="mx-auto w-full max-w-7xl grow px-8 pt-20.5 pb-8 text-sm md:px-16 md:pt-26 md:pb-12 md:text-base"
		id="content"
	>
		{@render children()}
	</main>

	<Footer />
</div>
