<script lang="ts">
    import linkedIn from '$lib/assets/icons/linkedin.png';
	import gitHub from '$lib/assets/icons/gitHub.png';
    import { ArrowUp, Mail, Phone } from '@lucide/svelte';
    import { mainLinks } from '$lib/assets/sitemap';
    import {MediaQuery} from "svelte/reactivity";

    interface socialMediaType {
        url: string,
        src: string,
        alt: string
    }

    const socialMedias = [
        {
            url: "https://github.com/Aurore-Dimech",
            src: gitHub,
            alt: "GitHub",
        },
        {
            url: "https://www.linkedin.com/in/aurore-dimech",
            src: linkedIn,
            alt: "LinkedIn",
        },
    ]

    const isDesktop = new MediaQuery("(min-width: 768px)");
</script>

{#snippet socialMedia(link: socialMediaType)}
    <li class="hover:ring-3 hover:border-ring hover:ring-ring/50 w-fit outline-none transition-all focus-within:ring-3 border border-transparent focus-within:border-ring focus-within:ring-ring/50 rounded-sm">
        <a href={link.url} target="_blank" class="focus:ring-0 focus:border-0 focus:outline-0 focus-visible:ring-0 focus-visible:border-0 focus-visible:outline-0" >
            <img src={link.src} alt={link.alt} class="h-10 md:h-12 " />
        </a>
    </li>
{/snippet}

<div class="rounded-full p-1 border border-ring/70 bg-ring/30 group hover:bg-black focus-within:bg-black transition-all w-fit h-fit ml-auto mt-2 mb-6 mr-8 md:mr-16">
    <a href="#top" aria-label="Return to the top of the page" class="block w-fit h-fit rounded-full border border-black bg-white p-2">
        <ArrowUp size={48} strokeWidth={1.5} />
    </a>
</div>

<footer id="footer" class="text-sm md:text-base w-screen px-6 sm:px-10 md:px-12 py-5 md:py-6 flex justify-between border-t border-ring/70  shrink-0 overflow-hidden bg-white gap-6 flex-wrap">

    <div class="flex flex-col">
        <h2 class="font-italiana text-lg md:text-2xl pb-1">Site map:</h2>
        <ul class='pl-2 border-l border-ring/50 py-1 flex flex-col gap-2'>
            {#each mainLinks as link}
                <li>
                    <a class="underline-offset-4 hover:underline outline-none transition-all focus-visible:ring-3 border border-transparent bg-clip-padding focus-visible:border-ring focus-visible:ring-ring/50 focus-visible:underline p-1 rounded-sm" href={link.url}>{link.name}</a>
                </li>
            {/each}
        </ul>
    </div>

    <div class="flex flex-col">
        <h2 class="font-italiana text-lg md:text-2xl pb-1">Contact:</h2>
        <ul class="pl-2 border-l border-ring/50 py-1 flex flex-col gap-2">
            <li>
                <a href="mailto:aurore.dimech@gmail.com" class="flex gap-1 items-center underline-offset-4 hover:underline outline-none transition-all focus-visible:ring-3 border border-transparent bg-clip-padding focus-visible:border-ring focus-visible:ring-ring/50 focus-visible:underline p-1 rounded-sm">
                    <Mail strokeWidth={1.5} size={isDesktop.current ? 20 : 18} />
                    aurore.dimech@gmail.com
                </a>
            </li>
            <li>
                <a href="tel:+33786878914" class="flex gap-1 items-center underline-offset-4 hover:underline outline-none transition-all focus-visible:ring-3 border border-transparent bg-clip-padding focus-visible:border-ring focus-visible:ring-ring/50 focus-visible:underline p-1 rounded-sm">
                    <Phone strokeWidth={1.5} size={isDesktop.current ? 20 : 18} />
                    +33 (0)7 86 87 89 14
                </a>
            </li>
        </ul>
    </div>

    <div class="flex flex-col">
        <h2 class="font-italiana text-lg md:text-2xl pb-1">Find me here:</h2>
        <ul class="pl-2 border-l border-ring/50 py-1 grayscale flex flex-col gap-2">
            {#each socialMedias as link}
                {@render socialMedia(link)}
            {/each}
        </ul>
    </div>
</footer>