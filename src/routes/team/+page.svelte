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
			name: 'Dr. Gangbing Song',
			title: 'Board Member & Researcher',
			image: 'profile-song.jpg',
			linkedinURL: 'https://www.me.uh.edu/faculty/song-gangbing',
			description: ''
		},
		{
			name: 'Dr. Dell Doyle',
			title: 'Director, Research',
			image: 'profile-dell-doyle.jpeg',
			linkedinURL: 'https://www.linkedin.com/in/delldoyle/',
			description:
				'Dell Doyle is a seasoned leader with nearly 15 years of experience driving innovation and collaboration in the plastics industry. As the Application Technology Expert for Dow Chemical’s North American Pipe team, he has spearheaded groundbreaking research in composite materials and resin development, earning multiple industry awards. A passionate advocate for advancing engineering, Dell excels in building high-performing teams and leveraging AI to accelerate research and optimize material design. His strategic leadership and commitment to innovation continue to shape the future of the industry.'
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
				'Nicholas holds an MS in Aerospace Engineering with expertise in Control Systems and Dynamics. His work focuses on airfoil stability, flutter prediction, and multidisciplinary optimization. As a contractor with ARCTOS through the Air Force Research Laboratory, he leverages tools like ESP, ASTROS, and Nastran to advance aerospace innovation, with a growing focus on applying AI to implement cutting-edge research in controls and aerospace systems.'
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
			title: 'Researcher, Sales Education',
			image: 'profile-skye-binion.jpg',
			linkedinURL: 'https://www.linkedin.com/in/skye-binion/',
			description:
				'Skye Binion is the Institute Manager at the Stephen Stagner Sales Excellence Institute, University of Houston. She oversees student development, mentors Key Accounts teams, and manages corporate partnerships to advance sales strategies. Currently pursuing a Master of Finance specializing in Financial Planning and Wealth Management, Skye combines her professional and academic expertise to shape the next generation of sales leaders.'
			// description:
			// 	'Skye Binion is the Institute Manager at the Stephen Stagner Sales Excellence Institute, where she mentors students, leads Key Accounts teams, and manages corporate partnerships. She is also pursuing a Master of Finance to further her expertise in financial planning and sales leadership.'
		},
		{
			name: 'David Johns',
			title: 'Researcher, Sales Education & Finance Education',
			image: 'profile-david.png',
			linkedinURL: 'https://www.linkedin.com/in/david-johns-18311b78/',
			description: ''
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
						class="wrap flex transform flex-col overflow-hidden rounded-lg bg-white shadow-lg transition duration-300 hover:scale-105 sm:flex-row"
					>
						<img
							src={member.image}
							alt={member.name}
							class="h-72 w-full object-cover object-center sm:h-auto sm:w-48"
						/>
						<!-- member-content -->
						<div class="flex flex-1 flex-col p-4">
							<div>
								<div
									class="mb-2 flex flex-col items-start justify-between sm:flex-row sm:items-center"
								>
									<h3 class="text-xl font-bold text-gray-800">{member.name}</h3>
									<div class="flex space-x-3">
										{#if member?.githubURL}
											<a href="/" class="text-blue-500 hover:text-blue-700">
												<IconGithub />
											</a>
										{/if}
										<a href={member.linkedinURL} class="text-blue-500 hover:text-blue-700">
											<IconLinkedIn />
										</a>
									</div>
								</div>
								<p class="mt-1 text-sm text-zinc-600">{member.title}</p>
							</div>
							<p class="mt-2 text-sm text-zinc-500">{member.description}</p>
						</div>
					</div>
				{/each}
			</div>
		</section>
	</section>
	<Spacer />
</main>
