<script lang="ts">
    import {Button, type ButtonProps} from "$lib/components/ui/button";
    import type {Snippet} from "svelte";
    import {cn} from "$lib/utils";
    import { page } from '$app/state';
    // import {faPaw} from "@fortawesome/free-solid-svg-icons";
    // import {Fa} from "svelte-fa";

    interface Props extends ButtonProps {
        children: Snippet
        class?: string;
    }

    let {children, class: className = '', ...other}: Props = $props();

    const url = $derived(page.url.pathname)

    function isActive() {
        if (other.href === "/") return url === "/";
        return url.startsWith(other.href!);
    }

</script>

<div class={"inline relative"}>

    <Button
            {...other}
            variant="link"
            class={cn(
            "text-base md:text-lg font-mazzard font-medium px-2! lg:px-4! underline-offset-4 focus:underline focus-within::underline hover:underline focus:outline-black focus-within::outline-black hover:outline-black focus:outline focus-within::outline",
            className,
            isActive() && "bg-ring/20 border-ring/70"
        )}
    >
        {@render children()}
    </Button>

</div>