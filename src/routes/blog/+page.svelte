<script>
	import BlogPost from '$lib/slices/BlogPost.svelte';
	import Spacer from '$lib/slices/Spacer.svelte';
	export const prerender = true;

	const posts = [
		{
			title: 'The Future of AI in Healthcare',
			date: '2023-04-01',
			author: 'John Smith',
			image: '/images/blog/ai-in-healthcare.jpg',
			description:
				'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed euismod, nisl nec ultricies...'
		},
		{
			title: 'The Future of AI in Healthcare',
			date: '2023-04-01',
			author: 'John Smith',
			image: '/images/blog/ai-in-healthcare.jpg',
			description:
				'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed euismod, nisl nec ultricies...'
		},
		{
			title: 'The Future of AI in Healthcare',
			date: '2023-04-01',
			author: 'John Smith',
			image: '/images/blog/ai-in-healthcare.jpg',
			description: 'Lorem ipsum dolor sit amet'
		}
	];
</script>

<div class="min-h-[calc(100vh-124px)]">
	<div class="border-b-2">
		<section class="container mx-auto border-x-2 border-zinc-800 sm:max-w-[1200px]">
			<div class="px-6 py-12">
				<code class="text-zinc-400">the publication office —</code>
				<h1 class="mt-6 mb-8 text-6xl font-bold">Blog</h1>
				<p class="text-xl text-zinc-500">Open Communcation, Open Accountability, Open Success.</p>
			</div>
		</section>
	</div>

	<Spacer />

	<section class="border-y-2 border-zinc-800">
		<div class="mx-auto border-x-2 border-zinc-800 sm:max-w-[1200px]">
			<div class="p-6">
				<h1 class="text-2xl">More thoughts soon.</h1>
			</div>
			<!-- Blog Posts -->
			<!-- {#each post} -->
			<!-- <BlogPost /> -->
		</div>
	</section>
</div>
