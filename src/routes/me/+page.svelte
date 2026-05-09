<script>
	import Breadcrumb from "$lib/components/layouts/Breadcrumb.svelte";
	import TextLink from "$lib/components/TextLink/TextLink.svelte";
	import Timeline from "$lib/components/Timeline/Timeline.svelte";
	import point from "$lib/assets/point.svg"
	import { base } from "$app/paths";
	import Hero from "$lib/components/layouts/hero/Hero.svelte";
	
</script>

<Hero>
	{#snippet description()}
		My education and my work experience taught me a lot of skills and competences. However, some of them also come from other activities I do in my free time !
	{/snippet}
</Hero>

<section class="py-6 md:py-10 border-t border-ring-50 ">
    <h2 class="font-italiana text-2xl md:text-4xl pb-4 md:pb-6">Sports</h2>

	<ul class="list-disc pl-4 pb-2">
		<li>Daily practice of dancing</li>
		<li>Weekly practice of climbing</li>
		<li>Occasional practice of fitness</li>
	</ul>

	<p>Ballet and karate are two sports that I practiced weekly and competed in for more than 10 years. Even though I stopped some time ago, I am interested in going back to those in the near future.</p>
</section>

<section class="py-6 md:py-10 border-t border-ring-50 ">
    <h2 class="font-italiana text-2xl md:text-4xl pb-4 md:pb-6">Hobbies</h2>

	<div class="flex flex-col gap-2">
        <div>
            <div class="flex items-center gap-2">
                <img src={point} alt="" class="size-6 md:size-8"/>
                <h3 class="font-italiana text-lg md:text-2xl">Reading</h3>
            </div>
			<div class="py-4 flex flex-col gap-1.5">
				<p>Reading is one of my favorite activities since I was a child.</p>
				<p>At first, I tended to mainly go towards <span class="font-semibold">fantasy</span>. From then I made my way slowly towards other genres, such as <span class="font-semibold">romance, classic Literature, novels and essays</span>. Nowadays, in addition to my other reading material, I quite often read <span class="font-semibold">scientific articles</span> on websites such as <TextLink href='https://pubmed.ncbi.nlm.nih.gov/'>PubMed</TextLink>.</p>
				<p>I read mostly in <span class="font-semibold">English and French</span>. At the moment, my favorite novel is <span class="font-semibold">Pride and Prejudice by Jane Austen</span> and my favorite series is <span class="font-semibold">A Chorus of Dragons by Jenn Lyons</span>.</p>
			</div>
		</div>
        <div>
            <div class="flex items-center gap-2">
                <img src={point} alt="" class="size-6 md:size-8"/>
                <h3 class="font-italiana text-lg md:text-2xl">Manual & artistic activities</h3>
            </div>
			<div class="py-4 flex flex-col gap-4">
				<div>
					<p class="pb-1.5">As stated in my soft skills, I am a creative person at heart. I've mainly been <span class="font-semibold">dancing and drawing</span> for years, but I like to try a lot of different mediums. For example, I have done some <span class="font-semibold">painting, sewing, wood carving, wire sculpture, or even linocuts</span>.</p>
					<p>My recent passions are <span class="font-semibold">weaving alpha patterns, knitting, and crocheting</span>.</p>
				</div>

				<div class="flex flex-wrap gap-4 items-center justify-center">
					<div class="flex justify-center grow flex-1 min-w-54 max-w-95">
						<img src={`${base}/arts/alpha.png`} alt="weaved bracelet with a drawing of a torch in it" class="object-center object-cover" />
					</div>
					<div class="flex justify-center grow flex-1 min-w-54 max-w-95">
						<img src={`${base}/arts/litho.jpg`} alt="linocut of a simple character in the light" class="object-center object-cover" />
					</div>
					<div class="flex justify-center grow flex-1 min-w-54 max-w-95">
						<img src={`${base}/arts/crochet.jpg`} alt="a crocheted rose" class="object-center object-cover" />
					</div>
				</div>

			</div>
		</div>

	</div>

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