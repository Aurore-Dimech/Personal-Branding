<script>
	import Breadcrumb from "$lib/components/layouts/Breadcrumb.svelte";
	import Timeline from "$lib/components/Timeline/Timeline.svelte";

</script>

<Breadcrumb page={"Certifications"} />

<section class="mx-auto flex flex-col items-center gap-3 py-8 md:px-20 md:py-12">
	<h1 class="text-center font-italiana text-4xl md:text-6xl">Certifications</h1>
	<p class="text-center">
		The certifications I obtained during my school years can be used to attest and verify the skills I learned and applied to my projects. You can find them below.
	</p>
</section>

<Timeline>
	{#snippet title()}
		Master's Degree in Web Engineering and Digital Innovation
	{/snippet}
	{#snippet dates()}
		2025 – present
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
		<ul class="flex flex-wrap gap-1 pb-2">
			<li>Full-Stack Development | </li>
			<li>Online Deployment | </li>
			<li>Computer Science | </li>
			<li>Software Architecture | </li>
			<li>Cybersecurity | </li>
			<li>Cloud Computing | </li>
			<li>CI-CD</li>
		</ul>
		<p>
			Majoring in DevOps and Backend Development
		</p>
	{/snippet}
</Timeline>

<Timeline>
	{#snippet title()}
		Bachelor's Degree in Digital Project Management
	{/snippet}
	{#snippet dates()}
		2023 – 2025
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
		<ul class="flex flex-wrap gap-1 pb-2">
			<li>Project Management | </li>
			<li>Full-Stack Development | </li>
			<li>Databases | </li>
			<li>Agile Methodologies | </li>
			<li>UX/UI Design | </li>
			<li>Networking | </li>
			<li>AI | </li>
		</ul>
		<p>
			Majored in Web Development and Digital Innovations
		</p>
		<p>
			Majored with highest honors and was the valedictorian
		</p>
	{/snippet}
</Timeline>

<Timeline>
	{#snippet title()}
		Bachelor's Degree in Psychology
	{/snippet}
	{#snippet dates()}
		2020 – 2023
	{/snippet}
	{#snippet tags()}
		<div class="w-fit rounded-full border border-black px-3 py-1">
			<p>Université Paris VIII Saint-Denis</p>
		</div>
		<div class="w-fit rounded-full border border-black px-3 py-1">
			<p>France, Paris</p>
		</div>
	{/snippet}

	{#snippet content()}
		<ul class="flex flex-wrap gap-1 pb-2">
			<li>Communication | </li>
			<li>Management | </li>
			<li>Labor Laws | </li>
			<li>Clinical Psychology | </li>
			<li>Scientific Research | </li>
			<li>Neuropsychology | </li>
			<li>Gerontology | </li>
		</ul>
		<p>
			Majored in Neurosciences and Psychosocial Risks
		</p>
		<p>
			Majored with highest honors and was the valedictorian
		</p>
	{/snippet}
</Timeline>

<Timeline>
	{#snippet title()}
		PIX Certification
	{/snippet}
	{#snippet dates()}
		2020
	{/snippet}
	{#snippet tags()}
		<div class="w-fit rounded-full border border-black px-3 py-1">
			<p>Université Paris VIII Saint-Denis</p>
		</div>
		<div class="w-fit rounded-full border border-black px-3 py-1">
			<p>France, Paris</p>
		</div>
	{/snippet}

	{#snippet content()}
		<ul class="flex flex-wrap gap-1 pb-2">
			<li>Online communication | </li>
			<li>Digital creation | </li>
			<li>Cybersecurity | </li>
			<li>Digital environment | </li>
		</ul>
		<p>
			Was deemed "advanced level 1" with a score of 595
		</p>
	{/snippet}
</Timeline>

<Timeline>
	{#snippet title()}
		High School Degree
	{/snippet}
	{#snippet dates()}
		2017 - 2020
	{/snippet}
	{#snippet tags()}
		<div class="w-fit rounded-full border border-black px-3 py-1">
			<p class="italic">Lycée de la Vallée de Chevreuse</p>
		</div>
		<div class="w-fit rounded-full border border-black px-3 py-1">
			<p>France, Paris</p>
		</div>
	{/snippet}

	{#snippet content()}
		<p>
			Majored in Cinema and Audiovisual
		</p>
		<p>
			Majored with highest honors
		</p>
	{/snippet}
</Timeline>
