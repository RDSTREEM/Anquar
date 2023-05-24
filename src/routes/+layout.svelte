<script lang="ts">
	// The ordering of these imports is critical to your app working properly
	import '../theme.postcss';
	// If you have source.organizeImports set to true in VSCode, then it will auto change this ordering
	import '@skeletonlabs/skeleton/styles/skeleton.css';
	// Most of your app wide CSS should be put in this file
	import '../app.postcss';

	import {
		AppBar,
		AppShell,
		Drawer,
		drawerStore,
		type DrawerSettings
	} from '@skeletonlabs/skeleton';
	import Navigation from '$lib/components/navigation.svelte';

	// Navigation Drawer Opener
	const date = new Date();
	const drawerSettings: DrawerSettings = {
		width: 'w-[45%] lg:w-[25%]'
	};

	const openNav = () => {
		drawerStore.open(drawerSettings);
	};
</script>

<Drawer>
	<Navigation />
</Drawer>

<AppShell>
	<svelte:fragment slot="header">
		<AppBar>
			<svelte:fragment slot="lead">
				<button class="block md:hidden" on:click={openNav}>
					<svg
						style="color: white"
						height="32px"
						id="Layer_1"
						version="1.1"
						viewBox="0 0 32 32"
						width="32px"
						xml:space="preserve"
						xmlns="http://www.w3.org/2000/svg"
						xmlns:xlink="http://www.w3.org/1999/xlink"
					>
						<path
							d="M4,10h24c1.104,0,2-0.896,2-2s-0.896-2-2-2H4C2.896,6,2,6.896,2,8S2.896,10,4,10z M28,14H4c-1.104,0-2,0.896-2,2 s0.896,2,2,2h24c1.104,0,2-0.896,2-2S29.104,14,28,14z M28,22H4c-1.104,0-2,0.896-2,2s0.896,2,2,2h24c1.104,0,2-0.896,2-2 S29.104,22,28,22z"
							fill="white"
						/>
					</svg>
				</button>
			</svelte:fragment>
			<header class="md:text-left text-center text-xl text-secondary-400">
				Anquar Management Solutions
			</header>
			<svelte:fragment slot="trail">
				<div class="hidden md:block pr-2">
					<div class="flex gap-8">
						<a class="btn variant-ringed-primary hover:variant-ghost-primary" href="/">Home</a>
						<a href="/services" class="btn variant-ringed-primary hover:variant-ghost-primary">
							Services
						</a>
						<a href="/directory" class="btn variant-ringed-primary hover:variant-ghost-primary">
							Business Directory
						</a>
						<a href="/about" class="btn variant-ringed-primary hover:variant-ghost-primary">
							About
						</a>
					</div>
				</div>
			</svelte:fragment>
		</AppBar>
	</svelte:fragment>
	<main class="container h-full mx-auto flex justify-center items-center mb-8">
		<slot />
	</main>
	<svelte:fragment slot="pageFooter">
		<div
			class="bg-surface-800 text-center min-h-[4rem] flex flex-col gap-2 p-2 items-center justify-center"
		>
			<p>Anquar Management Solutions</p>
			<p>Nurturing Business, Entrepreneurial and Leadership mindset.</p>
			<p>
				Copyright &copy; Anquar {date.getFullYear()}
			</p>
		</div>
	</svelte:fragment>
</AppShell>
