<script lang="ts">
	import IconGithub from '$lib/icons/IconGithub.svelte';
	import IconLinkedIn from '$lib/icons/IconLinkedIn.svelte';
	import IconX from '$lib/icons/IconX.svelte';
	import Spacer from '$lib/slices/Spacer.svelte';

	const teamMembers = [
		{
			name: 'Daniel Johns',
			title: 'President & Founder',
			image: 'profile-daniel-johns.jpeg',
			linkedinURL: 'https://www.linkedin.com/in/daniel-johns-a41403117/',
			description:
				'Daniel Johns is the driving force behind the Whole Human eXperience. With a background in aerospace engineering and a passion for innovation, he has been instrumental in shaping the company’s mission and strategy. Daniel’s expertise in AI and technology has been crucial in developing the company’s cutting-edge solutions. He is dedicated to using technology to improve the lives of individuals and communities.'
		},
		{
			name: 'Dr. Dell Doyle',
			title: 'Director, Research',
			image: 'profile-dell-doyle.jpeg',
			linkedinURL: 'https://www.linkedin.com/in/delldoyle/',
			description:
				'Daniel Johns is the driving force behind the Whole Human eXperience. With a background in aerospace engineering and a passion for innovation, he has been instrumental in shaping the company’s mission and strategy. Daniel’s expertise in AI and technology has been crucial in developing the company’s cutting-edge solutions. He is dedicated to using technology to improve the lives of individuals and communities.'
		},
		{
			name: 'Erik Kelly',
			title: 'Director, Engineering',
			image: 'profile-erik-kelly.jpeg',
			linkedinURL: 'https://www.linkedin.com/in/erik-kelly-36820a7/',
			description:
				'Erik Kelly, Director of Engineering at SaraWorks, specializes in the development and management of cloud-based multi-tenant SaaS solutions. With over 25 years of experience in Microsoft technologies, he leads a high-performing agile development team delivering mission-critical applications for government agencies nationwide.'
		},

		{
			name: 'Nicholas Tijerina',
			title: 'Researcher, Aerospace Engineering and Controls',
			image: 'profile-nick.jpeg',
			linkedinURL: 'https://www.linkedin.com/in/nicholas-tijerina-64b664208/',
			description:
				'Nick Tijerina is a dedicated professional with a strong background in the oil and gas industry, currently serving as a Field Specialist at Baker Hughes. He holds a Bachelor of Science in Mechanical Engineering from Texas A&M University. Nick’s expertise includes wellbore intervention, production optimization, and equipment maintenance. He is recognized for his problem-solving skills and commitment to safety and efficiency in field operations.'
		},
		{
			name: 'Caspian Harvey',
			title: 'Researcher, Education & Materials Engineering',
			image: 'profile-caspian-harvey.png',
			linkedinURL: 'https://www.linkedin.com/in/caspianharvey/',
			description:
				'Caspian Harvey brings a unique blend of technical expertise and educational experience to the team. With a Bachelor of Science in Mechanical Engineering and extensive experience in STEM education, he specializes in materials engineering research. His diverse background in engineering, computer programming, and teaching enables him to approach technical challenges with both analytical precision and clear communication skills.'
		},
		{
			name: 'Skye Binion',
			title: 'Researcher, Sales Euducation',
			image: 'profile-skye-binion.jpg',
			linkedinURL: 'https://www.linkedin.com/in/skye-binion/',
			description: `Skye Binion is an Institute Manager at the C.T. Bauer College of Business, University of Houston. In this role, she manages the Institute's students and leads and mentors the Key Accounts teams.`
		}
	];
</script>

<main class="min-h-[calc(100vh-124px)]">
	<div class="border-b-2">
		<section class="mx-auto border-x-2 border-zinc-800 sm:max-w-[1200px]">
			<div class="px-6 py-12">
				<code class="text-zinc-400">made of real —</code>
				<h1 class="mt-6 mb-8 text-6xl font-bold">Team</h1>
				<p class="text-xl text-zinc-500">Many Backgrounds—One Goal</p>
			</div>
		</section>
	</div>

	<Spacer />
	<section class="border-y-2 border-zinc-800">
		<section class="mx-auto border-x-2 border-zinc-800 py-12 sm:max-w-[1200px]">
			<div class="grid grid-cols-1 gap-6 px-6 md:grid-cols-2">
				{#each teamMembers as member}
					<div
						class="flex transform overflow-hidden rounded-lg bg-white shadow-lg transition duration-300 hover:scale-105"
					>
						<img
							src={member.image}
							alt={member.name}
							class="h-50 w-50 object-cover object-center"
						/>
						<div class="flex-1 p-4">
							<h3 class="text-xl font-bold text-gray-800">{member.name}</h3>
							<p class="mt-1 text-sm text-zinc-600">{member.title}</p>
							<p class="mt-2 text-sm text-zinc-500">{member.description}</p>
							<div class="mt-3 flex space-x-3">
								{#if member?.githubURL}
									<a href="/" class="text-blue-500 hover:text-blue-700">
										<IconGithub />
									</a>
								{/if}
								<a href={member.linkedinURL} class="text-blue-500 hover:text-blue-700">
									<IconLinkedIn />
								</a>
								<!-- <a href="/" class="text-blue-500 hover:text-blue-700">
									<IconX />
								</a> -->
							</div>
						</div>
					</div>
				{/each}
			</div>
		</section>
	</section>
	<Spacer />
</main>
