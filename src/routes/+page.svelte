<script>
	import { onMount } from 'svelte';

	// let startupMS = 0;

	onMount(() => {
		// startupMS = performance.now().toFixed(0);
	});

	const projects = [
		{
			name: 'Vite',
			description: 'The build tool for the web',
			stars: '69.6',
			logo: '/projects/vite.svg',
			github: 'https://github.com/vitejs/vite'
		},
		{
			name: 'Vitest',
			description: 'Next-generation test runner',
			stars: '13.5',
			logo: '/projects/vitest.svg',
			github: 'https://github.com/vitest-dev/vitest'
		}
		// Add more projects as needed
	];
</script>

<!-- Header -->

<!-- Hero Section -->
<section class="container mx-auto border-r-2 border-b-2 border-l-2 border-zinc-800">
	<div class="px-6 py-12">
		<code class="text-zinc-400">for the...</code>
		<h1 class="mt-6 mb-8 text-6xl font-bold">
			Whole<br />
			Human<br />
			EXperience<br />
			<!-- Next Generation Tooling for -->
		</h1>
		<p class="text-xl text-zinc-500">
			Our mission is to have AI better serve Humanity, by understanding Humanity.
		</p>
	</div>
</section>

<!-- Projects Section -->
<section class="py-20">
	<div class="container mx-auto px-6">
		<div class="mb-12 flex items-center gap-4">
			<span class="text-violet-400">01</span>
			<h2 class="text-4xl font-bold">Projects</h2>
		</div>
		<p class="mb-8 max-w-3xl text-zinc-300">
			We are the creators, maintainers, and contributors of some of the most critical infrastructure
			projects in the JavaScript ecosystem.
		</p>
		<code class="mb-8 block text-zinc-400">projects.json</code>

		<!-- <div class="grid grid-cols-1 gap-8 md:grid-cols-2 lg:grid-cols-4">
				{#each projects as project}
					<div
						class="rounded-xl border border-zinc-800 bg-black p-6 transition-colors hover:border-violet-500"
					>
						<img src={project.logo} alt={project.name} class="mb-4 h-12" />
						<h6 class="text-sm text-zinc-400">{project.description}</h6>
						<h3 class="mt-2 mb-4 text-2xl font-bold">{project.name}</h3>
						<div class="flex items-center justify-between">
							<div>
								<h5 class="font-bold">{project.stars}k</h5>
								<p class="text-sm text-zinc-400">GitHub stars</p>
							</div>
							<a href={project.github} target="_blank" rel="noopener noreferrer">
								<img src="/github-icon.svg" alt="GitHub" class="h-6" />
							</a>
						</div>
					</div>
				{/each}
			</div> -->
	</div>
</section>
