<script>
	import { Avatar } from '@skeletonlabs/skeleton';
</script>

<svelte:head>
	<title>Anquar | About</title>
</svelte:head>

<div class="grid gap-4 mt-4 place-items-center">
	<div class="card hover:card-hover text-justify p-8">
		Anquar Management Solutions is a business, management and leadership consultancy firm that
		provides state of the art training consultancy and research solutions for businesses from
		individuals to SMES, to corporations. Anquar Management Solutions is committed to provide state
		of the art solutions to help businesses and organizations to scale up to the next level.
		Training, Research and consultancy services at Anquar Management solutions focus on critical
		issues that play a vital role in enhancing the competitive position of businesses and
		organizations that could in return provide a sustainable competitive advantage for companies and
		organizations. Training, research and consultancy provided by Anquar Management Solutions
		include: strategy, marketing and sales, operations, leadership, innovation and entrepreneurship.
		<div class="mt-4 card grid grid-cols-3">
			<div class="p-4 card rounded-r-none">
				<header class="text-center mb-2 text-tertiary-400">Vision</header>
				To be a primer training, consultancy and research hub in areas of business management and leadership
				in Ethiopia and beyond by the year 2035!
			</div>
			<div class="p-4 card rounded-none">
				<header class="text-center mb-2 text-tertiary-400">Mission</header>
				To provide a state of the art, need based and problem solving training, consultancy and research
				service that could enhance competitiveness of organizations and companies.
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
		<div class="container flex">
			<a
				href="https://abebekebie.vercel.app/"
				class="card rounded-tr-none rounded-br-none p-8 grid hover:card-hover"
			>
				<div class="card-header text-center">Manager</div>
				<div class="flex gap-4 items-center">
					<Avatar background="variant-filled-primary" initials="AK" />
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
	<div class="p-4">
		<header class="text-center text-lg">Contact Us</header>
		<p>Gmail: <a href="mailto:girarchz@gmail.com">girarchz@gmail.com</a></p>
		<p>Phone Number: +25191870202</p>
		<p>
			Linkedin: <a href="https://www.linkedin.com/in/abebe-kebie-hunegnawu-884241223">
				@abebe-kebie
			</a>
		</p>
	</div>
</div>
