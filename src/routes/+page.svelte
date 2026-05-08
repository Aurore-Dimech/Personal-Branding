<script>
	import Breadcrumb from "$lib/components/layouts/Breadcrumb.svelte";
    import point from "$lib/assets/point.svg"
    import me from "$lib/assets/me.jpg"
	import TextLink from "$lib/components/TextLink/TextLink.svelte";
</script>

<Breadcrumb page={"Home"} />

<section class="mx-auto flex flex-col gap-3 items-center md:px-20 py-8 md:py-12">
    <h1 class="font-italiana text-4xl md:text-6xl text-center">Aurore Dimech</h1>
    <div class="-order-1 border border-black px-3 py-1 rounded-full">
        <h2>Full Stack Developer</h2>
    </div>
    <ul class="flex gap-1 flex-wrap items-center justify-center">
        <li>
            <p>French citizen |</p>
        </li>
        <li>
            <p>Paris, France |</p>
        </li>
        <li>
            <p>Driving Licence Category B</p>
        </li>
    </ul>

    <p class="text-center my-4">
        Hello there! I’m Aurore, a full stack developer who specializes in digital accessibility, especially to improve the experience of blind people. I work with public and private institutions and companies such as <TextLink href="https://grauw.fr/">GRAUW.</TextLink>  to ensure that everyone can use the websites and applications they could need or want.
    </p>

    <div class="rounded-full p-1 border border-ring/70 bg-ring/30 group hover:bg-black focus-within:bg-black transition-all">
        <a
            href="mailto:aurore.dimech@edu.devinci.fr"
            class="block rounded-full px-4 py-2 border border-black bg-white group-hover:underline group-focus:underline group-focus-within:underline focus-visible:outline-0 underline-offset-4 outline-0 text-base md:text-lg"
        >
            Contact me!
        </a>
    </div>
</section>

<section class="py-6 md:py-10 border-t border-ring-50 ">
    <h2 class="font-italiana text-2xl md:text-4xl pb-4 md:pb-6">Presentation</h2>
    <div class="flex flex-col sm:flex-row gap-10 md:gap-12 justify-between">
        <div class="flex flex-col gap-4">
            <p>My name is Aurore, and I am a 23-year-old web developer specialized in backend development and digital accessibility. <br> My goal is to help create and upgrade websites and applications in order to optimize them and make them more user-friendly.</p>
            <p>I am currently employed as a Full Stack Developer Apprentice at <TextLink href="https://grauw.fr/">GRAUW.</TextLink> while pursuing a Master's Degree in Web Engineering and Digital Innovation.</p>
            <p>Let's work together in the near future!</p>
            <div class="rounded-full p-1 border border-ring/70 bg-ring/30 group hover:bg-black focus-within:bg-black transition-all mx-auto">
                <a
                    href="mailto:aurore.dimech@edu.devinci.fr"
                    class="block rounded-full px-4 py-2 border border-black bg-white group-hover:underline group-focus:underline group-focus-within:underline focus-visible:outline-0 underline-offset-4 outline-0 text-base md:text-lg"
                >
                    Contact me!
                </a>
            </div>
        </div>
        <img src={me} alt="" class="mx-auto md:mx-0 w-full sm:w-1/3 max-w-2xs object-contain object-top -order-1 sm:order-last" />
    </div>
</section>

<section class="py-6 md:py-10 border-t border-ring-50">
    <h2 class="font-italiana text-2xl md:text-4xl pb-4 md:pb-6">Skills</h2>

    <div class="flex flex-col gap-2">
        <div>
            <div class="flex items-center gap-2">
                <img src={point} alt="" class="size-6 md:size-8"/>
                <h3 class="font-italiana text-lg md:text-2xl">Soft Skills</h3>
            </div>
            <ul class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-1.5 list-disc list-inside p-4  ">
                <li>Hardworking</li>
                <li>Detail-oriented</li>
                <li>Organized</li>
                <li>Self-reliant</li>
                <li>Good team player</li>
                <li>Adaptive</li>
                <li>Patient</li>
                <li>Good listening qualities</li>
                <li>Creative</li>
                <li>Curious</li>
                <li>Open-minded</li>
                <li>Eager to learn and grow</li>
            </ul>
        </div>
    
        <div>
            <div class="flex items-center gap-2">
                <img src={point} alt="" class="size-6 md:size-8"/>
                <h3 class="font-italiana text-lg md:text-2xl">Hard Skills</h3>
            </div>
            <ul class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-1.5 list-disc list-inside p-4 ">
                <li>HTML</li>
                <li>CSS</li>
                <li>JavaScript</li>
                <li>PHP</li>
                <li>Python</li>
                <li>Node.js</li>
                <li>WordPress</li>
                <li>Laravel</li>
                <li>Tailwind CSS</li>
                <li>Svelte</li>
                <li>MySQL</li>
                <li>Figma</li>
            </ul>
        </div>
    </div>
</section>

<section class="py-6 md:py-10 border-t border-ring-50 ">
    <h2 class="font-italiana text-2xl md:text-4xl pb-4 md:pb-6">Foreign Languages</h2>

    <div class="flex flex-col gap-4">
        <div>
            <p> At the moment, I:</p>
            <ul class="list-disc list-inside">
                <li>am <span class="font-semibold">native French speaker</span></li>
                <li>have a level <span class="font-semibold">C1 in English</span> (TOEFL 2023)</li>
                <li>have a <span class="font-semibold">conversational Spanish</span>.</li>
            </ul>
        </div>
    
        <p>I maintain those levels by <span class="font-semibold">reading and watching works in foreign languages</span>, and by doing various <span class="font-semibold">trips abroad </span>in countries such as the United Kingdom or Spain.</p>
    
        <p>I plan to expand my knowledge by learning the <span class="font-semibold">French and British Sign Languages</span>, and by improving my Spanish abilities.</p>
    </div>
</section>

<section class="py-6 md:py-10 border-t border-ring-50 ">
    <h2 class="font-italiana text-2xl md:text-4xl pb-4 md:pb-6">Awards</h2>

    <div class="flex flex-col gap-2">
        <div class="flex flex-col gap-4 pb-4">
            <div>
                <div class="flex items-center gap-2">
                    <img src={point} alt="" class="size-6 md:size-8"/>
                    <div class="flex justify-between w-full items-center">
                        <h3 class="font-italiana text-lg md:text-2xl">A11y Paris</h3>
                        <p class="hidden sm:block text-right">September 2024 – June 2024</p>
                    </div>
                </div>
                <p class="block sm:hidden pl-8">September 2024 – June 2024</p>
            </div>
            <p><a href="https://www.a11yparis.org/" target="_blank" class="underline underline-offset-2 focus:font-semibold hover:font-semibold rounded-sm focus-visible:border-ring focus-visible:ring-ring/50 border border-transparent bg-clip-padding focus-visible:ring-3 transition-all outline-none">A11y Paris</a> is a <span class="font-semibold">French contest about digital accessibility</span>.</p>
            <p>With a designer and another full stack developer, we were tasked to <span class="font-semibold">upgrade the website of the Municipal library of Nice</span>,  and with a focus on <span class="font-semibold">digital accessibility</span>. Our work can be found <TextLink href="https://a11y-nice-iim.vercel.app/">here</TextLink>.</p>

            <div>
                <p>More precisely, I:</p> 
                <ul class="list-disc pl-4">
                    <li>actively participated in the <span class="font-semibold">creation of the mock-ups</span> to ensure it was <span class="font-semibold">compliant with accessibility standards</span>, especially in terms of contrast between colors, button labels, and component behaviors</li>
                    <li>complied with every <span class="font-semibold">RGAA criteria</span> to ensure usability of our product by everyone, with or without disabilities such as blindness</li>
                </ul>
            </div>

            <p>In the end, we were awarded the <span class="font-semibold">first places for design and digital conformity</span>, and we won the <span class="font-semibold">Jury’s prize</span>.</p>

        </div>

        <div class="flex flex-col gap-4">
            <div>
                <div class="flex items-center gap-2">
                    <img src={point} alt="" class="size-6 md:size-8"/>
                    <div class="flex justify-between w-full items-center">
                        <h3 class="font-italiana italic text-lg md:text-2xl">Concours Général</h3>
                        <p class="hidden sm:block text-right">September 2018 – June 2020</p>
                    </div>
                </div>
                <p class="block sm:hidden pl-8">September 2018 – June 2020</p>
            </div>
            <p>In France, the <span class="italic">Concours Général</span> is the <span class="font-semibold">most prestigious academic competition</span> held every year between high school students in almost all subjects taught in both general, technological and professional high schools. Students who show great ability in one field are selected to participate by their teachers and their school principal.</p>
            <p>During my <span class="italic">Première</span> (11th grade) and my <span class="italic">Terminale</span> (12th and final grade), I was chosen by my teachers  to take part in the “<span class="italic">Concours Général</span>” in <span class="font-semibold">French Literature and Philosophy</span>.</p>
        </div>
    </div>
</section>


