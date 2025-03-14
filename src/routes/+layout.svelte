<script lang="ts">
	import '../app.css';

	import Header from '$lib/components/layoutComponents/Header.svelte';
	import Footer from '$lib/components/layoutComponents/Footer.svelte';
	let { children } = $props();
</script>

<Header />

{@render children()}

<Footer />
