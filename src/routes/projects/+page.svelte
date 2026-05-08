<script>
	import Breadcrumb from '$lib/components/layouts/Breadcrumb.svelte';
	import Timeline from '$lib/components/Timeline/Timeline.svelte';
	import TextLink from '$lib/components/TextLink/TextLink.svelte';
</script>

<Breadcrumb page={'Projects'} />

<section class="mx-auto flex flex-col items-center gap-3 py-8 md:px-20 md:py-12">
	<h1 class="text-center font-italiana text-4xl md:text-6xl">Projects</h1>
	<p class="text-center">
		I gained a lot of experience throughout my school years and thank to my apprenticeships, during which I had the opportunity to participate in various projects.
	</p>
</section>

<section class="py-6 md:py-10 border-t border-ring-50 ">
    <h2 class="font-italiana text-2xl md:text-4xl pb-4 md:pb-6">Work projects</h2>

	<Timeline> 
		{#snippet title()}
			Full Stack Developer (2-year apprenticeship)
		{/snippet}
		{#snippet dates()}
			September 2025 – present
		{/snippet}
		{#snippet tags()}
			<div class="w-fit rounded-full border border-black px-3 py-1">
				<p>GRAUW.</p>
			</div>
			<div class="w-fit rounded-full border border-black px-3 py-1">
				<p>France, Paris</p>
			</div>
		{/snippet}

		{#snippet content()}
			<p class="pb-2"><TextLink href="https://grauw.fr/">GRAUW.</TextLink> offers to create websites, applications and digital software for a variety of clients.</p>
			<ul class="list-disc pl-4">
				<li>Creating an <TextLink href="https://health.nuzzly.fr/">AI chatbot</TextLink> to assist people on their animal’s issues and questions</li>
				<li>Developing complex databases for our projects and implementing them with custom REST APIs built with Laravel</li>
				<li>Deploying production ready websites and applications</li>
			</ul>
			<br>

			<div>
				
			</div>
		{/snippet}
	</Timeline>

	<Timeline> 
		{#snippet title()}
			Full Stack Developer (1-year apprenticeship)
		{/snippet}
		{#snippet dates()}
			September 2024 – September 2025
		{/snippet}
		{#snippet tags()}
			<div class="w-fit rounded-full border border-black px-3 py-1">
				<p>GRAUW.</p>
			</div>
			<div class="w-fit rounded-full border border-black px-3 py-1">
				<p>France, Paris</p>
			</div>
		{/snippet}

		{#snippet content()}
			<p class="pb-2"><TextLink href="https://grauw.fr/">GRAUW.</TextLink> offers to create websites, applications and digital software for a variety of clients.</p>
			<ul class="list-disc pl-4">
				<li>Created and improved web interfaces using Svelte and Tailwind CSS</li>
				<li>Developed optimized databases, database queries and REST APIs on projects with Laravel</li>
				<li>Updated WordPress projects to build reusable personalized components for clients’ pages</li>
			</ul>
			<br>
		{/snippet}
	</Timeline>

	<Timeline> 
		{#snippet title()}
			Research Internship (1-year internship)
		{/snippet}
		{#snippet dates()}
			September 2024 – September 2025
		{/snippet}
		{#snippet tags()}
			<div class="w-fit rounded-full border border-black px-3 py-1">
				<p>UMR CNRS MNHN 7179 MECADEV</p>
			</div>
			<div class="w-fit rounded-full border border-black px-3 py-1">
				<p>France, Paris</p>
			</div>
		{/snippet}

		{#snippet content()}
			<p class="pb-2">UMR CNRS MNHN 7179 MECADEV is a research laboratory focused on analyzing the adaptation mechanisms of living species in response to environmental changes. It is the result of a collaboration between the <span class="italic">Centre National de la Recherche Scientifique</span> (French National Centre for Scientific Research - the French State Research Organisation) and the <span class="italic">Musée National d’Histoire Naturelle</span> (National Museum of Natural History - the National Natural History Museum of France).</p>
			<ul class="list-disc pl-4">
				<li>Conducted research on the differences in cognitive strategies between male and female Grey Mouse Lemurs using the laboratory’s archives and my own experiments</li>
				<li>Learned to correctly manipulate Grey Mouse Lemurs focusing on animal wellness and protection</li>
				<li>Managed a team of 3 people to ensure the respect of the scientific process in the various laboratory’s experiments</li>
			</ul>
		{/snippet}
	</Timeline>
</section>

<section class="pt-6 md:pt-10 border-t border-ring-50 ">
    <h2 class="font-italiana text-2xl md:text-4xl pb-4 md:pb-6">School projects</h2>

	<Timeline> 
		{#snippet title()}
			Full Stack Developer (3-month project)
		{/snippet}
		{#snippet dates()}
			November 2025 – January 2026
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
			<ul class="list-disc pl-4">
				<li>
					Created a <TextLink href="https://patientvoice-frontend.onrender.com/">website</TextLink> back aiming to facilitate the experience of the clients of functional rehabilitation centers
				</li>
				<li>
					Designed and developed a relevant solution by analyzing the clients' needs
				</li>
				<li>
					Contacted disabled people to ask their opinion about their experience on our website and implemented their feedback
				</li>
			</ul>
		{/snippet}
	</Timeline>

	<Timeline> 
		{#snippet title()}
			Full Stack Developer (4-month project)
		{/snippet}
		{#snippet dates()}
			January 2024 – April 2024
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
			<ul class="list-disc pl-4">
				<li>
					Created a website back office and front office to map the organisations for the town hall
					of Villeneuve-La-Garenne (a city near Paris)
				</li>
				<li>
					Organized the GitHub repository and implemented securities to check the proper compliance
					of the <TextLink href="https://www.conventionalcommits.org/en/v1.0.0/">Conventional Commits</TextLink> specs
				</li>
				<li>Generated CRON Jobs in a Node.js and Express.js backend using node-cron</li>
			</ul>
		{/snippet}
	</Timeline>

	<Timeline> 
		{#snippet title()}
			Project Manager (4-month project)
		{/snippet}
		{#snippet dates()}
			September 2023 – December
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
			<ul class="list-disc pl-4">
				<li>
					Managed a team of 9 students (developers, designers, communication experts) to create the
					visual identity, marketing strategy and website of <TextLink href="https://nouvellrtorcy.fr/">Nouvell’R</TextLink>, a recycling depot
				</li>
				<li>
					Managed client’s weekly reviews to discuss the project’s progress and establish the next features to develop according to the schedule and the priorities
				</li>
				<li>Maintained a kanban board to keep a clear view of the website’s evolutions and organized the tasks’ distribution</li>
			</ul>
		{/snippet}
	</Timeline>

	<Timeline> 
		{#snippet title()}
			Research project on stress, health and welfare at work (1-year project)
		{/snippet}
		{#snippet dates()}
			September 2022 – September 2023
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
			<ul class="list-disc pl-4">
				<li>
					Analyzed the consequences of working remote on efficiency and workplace relationships
				</li>
				<li>
					Conducted thorough interviews with a variety of profiles
				</li>
				<li>Used scientific methods to analyse qualitative data and wrote a <TextLink href="/research/Evolution_des_relations_au_travail_et_du_sentiment_subjectif_defficacite_avec_le_teletravail.pdf">scientific article</TextLink> based on a bibliography</li>
			</ul>
		{/snippet}
	</Timeline>

	<Timeline> 
		{#snippet title()}
			Research project on lifespan psychology (1-year project)
		{/snippet}
		{#snippet dates()}
			September 2022 – September 2023
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
			<ul class="list-disc pl-4">
				<li>
					Studied the consequences of the use of social media on body image and self-esteem among men
				</li>
				<li>
					Created a valid online survey and gathered more than 200 answers
				</li>
				<li>Wrote a <TextLink href="/research/LES_EFFETS_RS_SUR_LESTIME_DE_SOI_ET_LA_REPRESENTATION_DU_CORPS_CHEZ_LES_HOMMES.pdf">scientific article</TextLink> using our conclusions and a detailed bibliography</li>
			</ul>
		{/snippet}
	</Timeline>

	<Timeline> 
		{#snippet title()}
			Field study in ergonomics (4-month project)
		{/snippet}
		{#snippet dates()}
			September 2022 – December 2022
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
			<ul class="list-disc pl-4">
				<li>
					Studied the administrative agents of the Identity-Vigilance Cell of the Bichat Hospital (Paris)
				</li>
				<li>
					Analyzed the working environment and material given to the staff
				</li>
				<li>Discussed in detail the opinions of the workers about their working conditions</li>
			</ul>
		{/snippet}
	</Timeline>
</section>
