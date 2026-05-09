<script lang="ts">
	import { cn } from "$lib/utils";
	import { Mail } from "@lucide/svelte";

    interface ContactProps {
        class?: string
    }

    const {class: className}: ContactProps = $props();
</script>
<div class={cn("rounded-full p-1 border border-ring/70 bg-ring/30 group hover:bg-black focus-within:bg-black transition-all", className)}>
    <a
        href="mailto:aurore.dimech@edu.devinci.fr"
        class="rounded-full px-4 py-2 min-h-fit border border-black bg-white font-medium group-hover:underline group-focus:underline group-focus-within:underline focus-visible:outline-0 underline-offset-4 outline-0 text-base md:text-lg flex items-center gap-2"
    >
        <Mail stroke-width={1.5} />
        Contact me!
    </a>
</div>