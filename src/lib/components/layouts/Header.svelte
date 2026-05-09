<script lang="ts">
    import {Sheet, SheetContent, SheetHeader, SheetTitle, SheetTrigger} from "$lib/components/ui/sheet/index"
    import { Menu } from '@lucide/svelte';
    import {page} from "$app/state";
	import {pushState} from "$app/navigation";
    import {MediaQuery} from "svelte/reactivity";
    import favicon from '$lib/assets/logo.svg';
    import { mainLinks } from '$lib/assets/sitemap';
    import Link from '$lib/components/layouts/nav/Link.svelte';
	import { resolve } from "$app/paths";
	import ContactButton from "../ContactButton/ContactButton.svelte";

    const isBurgerOpen = $derived(!!page.state.burgerOpen);

	const onOpenChangeBurger = (open: boolean) => {
        open ?
            pushState('', {
                burgerOpen: true
            }) :
            history.back();
    }

	const isDesktop = new MediaQuery("(min-width: 768px)");
</script>

{#snippet navLinks(className?: string)}
	<ul class={className}>
		{#each mainLinks as link}
			<Link href={link.url}>{link.name}</Link>
		{/each}
		<li>
			<ContactButton />
		</li>
	</ul>
	
{/snippet}

<div class="z-40 fixed top-0 bg-white">
    <ul class="flex justify-evenly items-center py-4 text-sm md:text-base text-center
        absolute -translate-y-150 focus:translate-y-0 focus:relative focus-within:translate-y-0 focus-within:relative hover:translate-y-0 hover:relative
    ">
            <li>
                <a href="#navbar" class="focus:underline hover:underline focus:outline-black outline-offset-4">Go to the navbar</a>
            </li>
            <li>
                <a href="#content" class="focus:underline hover:underline focus:outline-black outline-offset-4">Go to the main content</a>
            </li>
            <li>
                <a href="#footer" class="focus:underline hover:underline focus:outline-black outline-offset-4">Go to the footer</a>
            </li>
        </ul>

    <header class="w-screen px-6 sm:px-10 md:px-12 py-5 md:py-6 flex justify-between items-center border-b border-ring/70  shrink-0 overflow-hidden bg-white" >
    
        {#if !isDesktop.current}
            <Sheet
                    onOpenChange={onOpenChangeBurger}
                    open={isBurgerOpen}
            >
                <SheetTrigger class="z-10! block md:hidden">
                    <div class="p-1 block md:hidden size-6">
                        <Menu strokeWidth={1.5} />
                    </div>
        
                </SheetTrigger>
                <SheetContent side="left">
                    <SheetHeader>
                        <SheetTitle>
                            <a href={resolve("/")} class="inline-block w-fit outline-none transition-all hover:ring-3 hover:border-ring hover:ring-ring/50 focus-visible:ring-3 border border-transparent bg-clip-padding focus-visible:border-ring focus-visible:ring-ring/50 p-1 rounded-sm" aria-label="Go to homepage">
                                <img src={favicon} width="100" alt="Logo Aurore D.">
                            </a>
                        </SheetTitle>
                    </SheetHeader>
        
                    <div class="p-4 h-full flex flex-col">
                        <nav id="mobile-nav-link-list" class="flex flex-col gap-2 grow">
                            {@render navLinks('flex flex-col items-start gap-2')}
                        </nav>
                    </div>
        
        
                </SheetContent>
            </Sheet>
        {/if}

        <a href={resolve("/")} aria-label="Go to homepage" class="hover:ring-3 hover:border-ring hover:ring-ring/50 outline-none transition-all focus-visible:ring-3 border border-transparent bg-clip-padding focus-visible:border-ring focus-visible:ring-ring/50 p-1 rounded-sm">
            <img src={favicon} width="36" alt="Logo Aurore D">
        </a>

        <nav id="navbar" class="hidden md:block">
            {@render navLinks('flex gap-1 lg:gap-2 items-center')}
        </nav>
    </header>
</div>