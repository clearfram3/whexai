<script lang="ts">
	import '../app.css';
	import Navbar from '$lib/slices/Navbar.svelte';
	import Footer from '$lib/slices/Footer.svelte';

	let { children } = $props();
</script>

<Navbar />

{@render children()}

<Footer />
