<script>
	import Spacer from '$lib/slices/Spacer.svelte';
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
<!-- <section class="container mx-auto border-r-2 border-b-2 border-l-2 border-zinc-800">
	<div class="px-6 py-12">
		<code class="text-zinc-400">for the...</code>
		<h1 class="mt-6 mb-8 text-6xl font-bold">
			Whole<br />
			Human<br />
			EXperience<br />
		</h1>
		<p class="text-xl text-zinc-500">
			Our mission is to have AI better serve Humanity, by understanding Humanity.
		</p>
	</div>
</section> -->
<section class="border-b-2 border-zinc-800">
	<div class="mx-auto border-x-2 px-20 py-12 sm:max-w-[1200px]">
		<code class="text-zinc-500">the Whole Human eXperience</code>
		<h1 class="offside-regular mt-6 mb-8 text-7xl font-bold">whex ai</h1>
		<!-- <h1 class="mt-6 mb-8 text-6xl font-bold">
			Whole<br />
			Human<br />
			EXperience<br />
		</h1> -->
		<!-- <p class="text-xl text-zinc-500">
			Our mission is to have AI better serve Humanity, by understanding Humanity.
		</p> -->
	</div>
</section>

<Spacer />
<section class="border-y-2 border-zinc-800">
	<div class="mx-auto border-x-2 border-zinc-800 p-6 sm:max-w-[1200px]">
		<div class="mb-10 flex justify-between">
			<h2 class="text-2xl font-bold">who we are</h2>
			<span class="text-2xl text-violet-400">01</span>
		</div>

		<!-- <h2 class="mb-12 text-4xl">Serve the People</h2> -->

		<p class="mx-auto mb-8 max-w-4xl text-center text-2xl text-zinc-900">
			We are engineers, professors, aviation experts, lawyers, politicians, and, more than all
			those, <span class="italic">just</span> people who want to make the world a better place.
		</p>
	</div>
</section>

<Spacer />
<section class="border-y-2 border-zinc-800">
	<div class="mx-auto border-x-2 border-zinc-800 p-6 sm:max-w-[1200px]">
		<div class="mb-10 flex justify-between">
			<h2 class="text-2xl font-bold">what we believe</h2>
			<span class="text-2xl text-violet-400">02</span>
		</div>

		<!-- <h2 class="mb-12 text-4xl">Serve the People</h2>
		<h2 class="mb-12 text-4xl">Reality over Celebrity</h2>
		<h2 class="mb-12 text-4xl">Results over Fiction</h2> -->

		<p class="mx-auto mb-8 max-w-4xl text-center text-2xl text-zinc-900">
			We want a future that is <span class="italic">good</span> for our people and our planet.
			<br />We believe AI is not <span class="italic">the</span> future, but an essential part of it,
			so must understand it and steer for the good of humanity.
		</p>
	</div>
</section>

<Spacer />
<section class="border-y-2 border-zinc-800">
	<div class="mx-auto border-x-2 border-zinc-800 p-6 sm:max-w-[1200px]">
		<div class="mb-10 flex justify-between">
			<h2 class="text-2xl font-bold">what we do</h2>
			<span class="text-2xl text-violet-400">03</span>
		</div>

		<p class="mx-auto mb-8 max-w-4xl text-center text-2xl text-zinc-900">
			We build tools and frameworks that help shape AI development with human values at their core.
			Through research, education, and practical applications, we work to ensure AI systems are
			developed with a deep understanding of human needs, ethics, and real-world impact.
		</p>

		<!-- <h2 class="mb-12 text-4xl">Serve the People</h2> -->

		<!-- <p class="mx-auto mb-8 max-w-4xl text-xl text-zinc-900">
			We want a future that is <span class="italic">good</span> for our people and our planet. We believe
			AI is part of the future, not the future, so we want
		</p> -->
	</div>
</section>

<!-- <Spacer />

<section class="border-y-2 border-zinc-800">
	<div class="mx-auto border-x-2 border-zinc-800 p-6 sm:max-w-[1200px]">
		<div class="mb-6 flex justify-between">
			<h2 class="text-2xl font-bold">Research Initiatives</h2>
			<span class="text-2xl text-violet-400">02</span>
		</div>

		<div class="border-zinc-800">
			<h2 class="mb-12 text-3xl">.1 - Safety <span class="italic">in</span> Safety</h2>
			<p class="mb-8 text-xl text-zinc-900">
				We understand that AI is a powerful tool, but it can also be dangerous if not used
				correctly. What is eqaully dangerous is the safety work being done with and against AI.
				Safety training inherently leaks and we need to be able to trust the safety work being done.
			</p>

			<h2 class="mb-12 text-3xl">.2 - Safety <span class="italic">from</span> Safety</h2>
			<p class="mb-8 text-xl text-zinc-900">
				We understand that AI is a powerful tool, but it can also be dangerous if not used
				correctly. What is eqaully dangerous is the safety work being done with and against AI.
				Safety training inherently leaks and we need to be able to trust the safety work being done.
			</p>

			<h2 class="mb-12 text-3xl">.2 - interpretation framework</h2>
			<p class="mb-8 text-xl text-zinc-900">
				We understand that AI is a powerful tool, but it can also be dangerous if not used
				correctly. What is eqaully dangerous is the safety work being done with and against AI.
				Safety training inherently leaks and we need to be able to trust the safety work being done.
			</p>
		</div>
	</div>
</section> -->

<Spacer />
