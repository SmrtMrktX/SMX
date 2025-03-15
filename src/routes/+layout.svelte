<script lang="ts">
	import '../app.css';

	import Header from '$lib/components/layoutComponents/Header.svelte';
	let { children } = $props();
	import Footer from '$lib/components/layoutComponents/Footer.svelte';
</script>

<Header />

{@render children()}

<Footer />
