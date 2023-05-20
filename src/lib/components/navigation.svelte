<script>
	import { drawerStore } from '@skeletonlabs/skeleton';

	const closeNav = () => {
		drawerStore.close();
	};
</script>

<!-- svelte-ignore a11y-click-events-have-key-events -->
<div class="p-4 flex flex-col gap-2" on:click={closeNav}>
	<a
		class="btn variant-ringed-primary hover:variant-ghost-primary flex justify-center items-center p-4"
		href="/"
	>
		Home
	</a>
	<a
		class="btn variant-ringed-primary hover:variant-ghost-primary flex justify-center items-center p-4"
		href="/services"
	>
		Services
	</a>
	<a
		class="btn variant-ringed-primary hover:variant-ghost-primary flex justify-center items-center p-4"
		href="/about"
	>
		About
	</a>
</div>
