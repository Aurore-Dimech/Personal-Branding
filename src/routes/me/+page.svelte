<script>
	import Breadcrumb from "$lib/components/layouts/Breadcrumb.svelte";
	import Timeline from "$lib/components/Timeline/Timeline.svelte";

</script>

<Breadcrumb page={"Learn more about me"} />

<section class="mx-auto flex flex-col items-center gap-3 py-8 md:px-20 md:py-12">
	<h1 class="text-center font-italiana text-4xl md:text-6xl">Learn more about me</h1>
	<p class="text-center">
		//
	</p>
</section>

<section class="py-6 md:py-10 border-t border-ring-50 ">
    <h2 class="font-italiana text-2xl md:text-4xl pb-4 md:pb-6">Sports</h2>

	<ul class="list-disc pl-4 pb-2">
		<li>Daily practice of dancing</li>
		<li>Weekly practice of climbing</li>
		<li>Occasional practice of fitness</li>
	</ul>

	<p>Ballet and karate are two sports that I practiced daily and competed in for more than 10 years. Even though I stopped some time ago, I am interested in going back to those in the near future.</p>
</section>

<section class="py-6 md:py-10 border-t border-ring-50 ">
    <h2 class="font-italiana text-2xl md:text-4xl pb-4 md:pb-6">Hobbies</h2>

	<h3 class="font-italiana text-lg md:text-2xl">Reading</h3>
	<h3 class="font-italiana text-lg md:text-2xl">Manual activities</h3>
</section>

<section class="py-6 md:py-10 border-t border-ring-50 ">
    <h2 class="font-italiana text-2xl md:text-4xl pb-4 md:pb-6">Clubs</h2>

	<Timeline> 
		{#snippet title()}
			Class president
		{/snippet}
		{#snippet dates()}
			September 2025 – present
		{/snippet}
		{#snippet tags()}
			<div class="w-fit rounded-full border border-black px-3 py-1">
				<p>IIM Digital School</p>
			</div>
			<div class="w-fit rounded-full border border-black px-3 py-1">
				<p>France, Paris</p>
			</div>
		{/snippet}
		{#snippet content()}
			<p>I am <span class="font-semibold">class president of the Web Engineering and Digital Innovation class</span>, since September 2025</p>
		{/snippet}
	</Timeline>

	<Timeline> 
		{#snippet title()}
			Communication manager
		{/snippet}
		{#snippet dates()}
			September 2023 – September 2024
		{/snippet}
		{#snippet tags()}
			<div class="w-fit rounded-full border border-black px-3 py-1">
				<p>IIM Digital School</p>
			</div>
			<div class="w-fit rounded-full border border-black px-3 py-1">
				<p>France, Paris</p>
			</div>
		{/snippet}
		{#snippet content()}
			<p> I was the <span class="font-semibold">communication manager in the 404DeVinci</span>, one of IIM Digital School’s student organisations, from September 2023 to September 2024</p>
		{/snippet}
	</Timeline>

	<Timeline> 
		{#snippet title()}
			Co-president
		{/snippet}
		{#snippet dates()}
			September 2016 – September 2017
		{/snippet}
		{#snippet tags()}
			<div class="w-fit rounded-full border border-black px-3 py-1">
				<p class="italic">Collège Juliette-Adam</p>
			</div>
			<div class="w-fit rounded-full border border-black px-3 py-1">
				<p>France, Paris</p>
			</div>
		{/snippet}
		{#snippet content()}
			<p> I was the <span class="font-semibold">co-president of the art student organisation</span>  of my middle school, from September 2016 to September 2017</p>
		{/snippet}
	</Timeline>
</section>