<script>
	import { Avatar } from '@skeletonlabs/skeleton';
</script>

<svelte:head>
	<title>Anquar | About</title>
</svelte:head>

<div class="grid gap-4 mt-4">
	<div class="card hover:card-hover text-justify p-8 max-w-xl">
		Anquar Management Solutions is a business, management and leadership consultancy firm that
		provides state of the art training consultancy and research solutions for businesses from
		individuals to SMES, to corporations. Anquar Management Solutions is committed to provide state
		of the art solutions to help businesses and organizations to scale up to the next level.
		Training, Research and consultancy services at Anquar Management solutions focus on critical
		issues that play a vital role in enhancing the competitive position of businesses and
		organizations that could in return provide a sustainable competitive advantage for companies and
		organizations. Training, research and consultancy provided by Anquar Management Solutions
		include: strategy, marketing and sales, operations, leadership, innovation and entrepreneurship.
	</div>
	<div class="card p-8 grid hover:card-hover">
		<div class="card-header text-center">Manager</div>
		<div class="flex gap-4 items-center">
			<Avatar background="variant-filled-primary" initials="AK" />
			<p>Abebe Kebie, Certified Management Consultant</p>
		</div>
	</div>
	<div class="card p-8 grid hover:card-hover">
		<div class="card-header text-center">Website Developer</div>
		<div class="flex gap-4 items-center">
			<Avatar background="variant-filled-secondary" initials="NA" />
			<p>Nahom Abebe, Full Stack Sveltekit Developer</p>
		</div>
	</div>
</div>
