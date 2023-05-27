<script>
	import Contact from '$lib/components/contact.svelte';
	import { Avatar } from '@skeletonlabs/skeleton';
</script>

<svelte:head>
	<title>Anquar | About</title>
</svelte:head>

<div class="grid gap-4 mt-4 place-items-center">
	<div class="card hover:card-hover text-justify p-8 lg:max-w-none max-w-[350px]">
		<p class="mb-4">
			Anquar Management Solutions is a Business, Management and Leadership consultancy firm that
			provides state of the art Training, Consultancy and Research solutions for businesses from
			individuals to SMES to corporations.
		</p>
		<p class="mb-4">
			Anquar Management Solutions is committed to provide state of the art solutions to help
			businesses and organizations to scale up to the next level. Training, Research and consultancy
			services at Anquar Management solutions focus on critical issues that play a vital role in
			enhancing the competitive position of businesses and organizations that could in return
			provide a sustainable competitive advantage for companies and organizations.
		</p>
		<p>
			Training, Research and Consultancy provided by Anquar Management Solutions include: Strategy,
			Marketing and Sales, Operations, Leadership, Innovation and Entrepreneurship.
		</p>
		<div class="mt-4 card lg:grid lg:grid-cols-3">
			<div class="p-4 card rounded-r-none">
				<header class="text-center mb-2 text-tertiary-400">Vision</header>
				To be a primer Training, Consultancy and Research hub in areas of Business, Management, Leadership
				and Strategy in Ethiopia and beyond by the year 2035!
			</div>
			<div class="p-4 card rounded-none">
				<header class="text-center mb-2 text-tertiary-400">Mission</header>
				To provide a state of the art, need based and problem solving training, consultancy and research
				services that could enhance competitiveness of organizations and companies.
			</div>
			<div class="p-4 card rounded-l-none">
				<header class="text-center mb-2 text-tertiary-400">Values</header>
				<ul class="pl-8 list-disc">
					<li>Professionalism</li>
					<li>Continuous Professional Development</li>
					<li>Team Work</li>
					<li>Customer Centercity</li>
					<li>Quality</li>
					<li>Strategic Thinking</li>
					<li>Commitment</li>
				</ul>
			</div>
		</div>
	</div>
	<div>
		<p class="text-center text-xl pb-4">People</p>
		<div class="container lg:flex">
			<a
				href="/about/manager"
				class="card rounded-tr-none rounded-br-none p-8 grid hover:card-hover"
			>
				<div class="card-header text-center">Managing Director</div>
				<div class="flex gap-4 items-center">
					<Avatar background="variant-filled-primary" src="/photo_2023-05-24_08-23-38.jpg" />
					<div>
						<p>Abebe Kebie</p>
						<p class="italic font-light blur-[0.5px]">Certified Management Consultant</p>
					</div>
				</div>
			</a>
			<div class="card rounded-tl-none rounded-bl-none p-8 grid hover:card-hover">
				<div class="card-header text-center">Website Developer</div>
				<div class="flex gap-4 items-center">
					<Avatar background="variant-filled-secondary" initials="NA" />
					<div>
						<p>Nahom Abebe</p>
						<p class="italic font-light blur-[0.5px]">Fullstack Sveltekit Web Developer</p>
					</div>
				</div>
			</div>
		</div>
	</div>
	<Contact />
</div>
