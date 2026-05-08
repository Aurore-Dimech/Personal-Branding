<script lang="ts">
    import point from "$lib/assets/point.svg"
	import type { Snippet } from "svelte";

    interface TimelineProps {
        title: Snippet
        dates: Snippet
        tags: Snippet
        content: Snippet
    }

    const {
        title,
        dates,
        tags,
        content
    }: TimelineProps = $props()
</script>

<div class="flex flex-col gap-4 pb-4">

    <div>
        <div class="flex items-center gap-2">
            <img src={point} class="size-10 md:size-12" alt="" />
            <div class="flex w-full items-center justify-between gap-4">
                <h3 class="font-italiana text-lg md:text-2xl">{@render title()}</h3>
                <p class="text-right shrink-0 hidden md:block">{@render dates()}</p>
            </div>
        </div>
        <p class="block md:hidden shrink-0 pl-12">{@render dates()}</p>
    </div>

	<div class="flex gap-2 items-stretch">
		<div class="w-10 shrink-0 md:w-12">
			<div class="h-full border-l-2 border-dashed border-ring/30 mx-auto w-0"></div>
		</div>

		<div>
            <div class="flex gap-2 pb-4 flex-wrap">
                {@render tags()}
            </div>
			{@render content()}
		</div>
	</div>
</div>