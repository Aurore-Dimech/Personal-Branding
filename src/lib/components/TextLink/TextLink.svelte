<script lang="ts">
	import type { Snippet } from "svelte";

    interface TextLinkProps {
        href?: string
        children: Snippet
    }

    const {href, children}: TextLinkProps = $props()
</script>

{#if href}
    <a
        href={href}
        target="_blank"
        class="underline underline-offset-2 focus:font-semibold group-focus-within:font-semibold hover:font-semibold group-hover:font-semibold rounded-sm focus-visible:border-ring focus-visible:ring-ring/50 border border-transparent bg-clip-padding focus-visible:ring-3 transition-all outline-none"
    >
        {@render children()}
    </a>
    {:else}
    <span class="underline underline-offset-2 focus:font-semibold group-focus-within:font-semibold hover:font-semibold group-hover:font-semibold rounded-sm focus-visible:border-ring focus-visible:ring-ring/50 border border-transparent bg-clip-padding focus-visible:ring-3 transition-all outline-none"
    >
        {@render children()}
    </span>
{/if}
