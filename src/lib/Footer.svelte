<script lang="ts">
	import { page } from '$app/state';
</script>

<header class="w-full border-t-2 border-zinc-800 bg-white">
	<nav
		class="container mx-auto flex items-center justify-between border-x-2 border-zinc-800 px-6 py-4"
	>
		<a href="/" class="offside-regular flex items-center text-xl">
			<!-- <img src="/logo.svg" alt="Logo" class="h-8" /> -->
			WHeX ai
		</a>
		<ul class="flex space-x-8">
			<li>
				<a href="/" class="hover:text-violet-400" class:text-violet-400={page.url.pathname == '/'}
					>Home</a
				>
			</li>
			<li>
				<a
					href="/blog"
					class="hover:text-violet-400"
					class:text-violet-400={page.url.pathname == '/blog'}>Blog</a
				>
			</li>
			<li>
				<a
					href="/team"
					class="hover:text-violet-400"
					class:text-violet-400={page.url.pathname == '/team'}>Team</a
				>
			</li>
		</ul>
	</nav>
</header>
