<script lang="ts">
	import IconLinkedIn from '$lib/icons/IconLinkedIn.svelte';
	import Spacer from '$lib/slices/Spacer.svelte';

	const teamMembers = [
		{
			name: 'Jane Doe',
			title: 'Chief Executive Officer',
			// image: '/images/team/jane-doe.jpg',
			image: 'https://i.pravatar.cc/300',
			description: 'Visionary leader with 15 years of tech industry experience.'
		},
		{
			name: 'John Smith',
			title: 'Chief Technology Officer',
			// image: '/images/team/john-smith.jpg',
			image: 'https://i.pravatar.cc/300',
			description: 'Expert in cutting-edge software architecture and innovation.'
		},
		{
			name: 'Emily Chen',
			title: 'Head of Product Design',
			// image: '/images/team/emily-chen.jpg',
			image: 'https://i.pravatar.cc/300',
			description: 'Design thinking expert with a passion for user-centric solutions.'
		}
	];
</script>

<main class="min-h-[calc(100vh-124px)]">
	<div class="border-b-2">
		<section class="mx-auto border-x-2 border-zinc-800 sm:max-w-[1200px]">
			<div class="px-6 py-12">
				<code class="text-zinc-400">who we are —</code>
				<h1 class="mt-6 mb-8 text-6xl font-bold">Team</h1>
				<p class="text-xl text-zinc-500">Many Backgrounds—One Goal</p>
			</div>
		</section>
	</div>

	<Spacer />

	<section class="border-y-2 border-zinc-800">
		<section class="mx-auto border-x-2 border-zinc-800 py-12 sm:max-w-[1200px]">
			<div class="grid grid-cols-1 gap-8 px-6 md:grid-cols-2 lg:grid-cols-3">
				{#each teamMembers as member}
					<div
						class="transform overflow-hidden rounded-lg bg-white shadow-lg transition duration-300 hover:scale-105"
					>
						<img
							src={member.image}
							alt={member.name}
							class="h-64 w-full object-cover object-center"
						/>
						<div class="p-6">
							<h3 class="text-2xl font-bold text-gray-800">{member.name}</h3>
							<p class="mt-2 text-zinc-600">{member.title}</p>
							<div class="mt-4 flex space-x-4">
								<a href="/" class="text-blue-500 hover:text-blue-700">
									<IconLinkedIn />
								</a>
								<a href="/" class="text-blue-500 hover:text-blue-700">
									<IconLinkedIn />
								</a>
							</div>
						</div>
					</div>
				{/each}
			</div>
		</section>
	</section>

	<Spacer />
</main>
