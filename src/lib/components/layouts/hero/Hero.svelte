<script lang="ts">
	import { mainLinks } from "$lib/assets/sitemap";
	import type { Snippet } from "svelte";
	import Breadcrumb from "../Breadcrumb.svelte";
	import { page } from "$app/state";

    interface HeroProps {
        description: Snippet
    }

    const {description}: HeroProps = $props()

    const namePage = mainLinks.filter(link => link.url === page.url.pathname)[0].name
</script>


<Breadcrumb page={namePage} />

<section class="mx-auto flex flex-col items-center gap-3 py-8 md:px-20 md:py-12">
	<h1 class="text-center font-italiana text-4xl md:text-6xl">{namePage}</h1>
	<p class="text-center">
		{@render description()}
	</p>
</section>