<script lang="ts">
	import '../app.css';

	import Header from '$lib/components/layoutComponents/Header.svelte';
	let { children } = $props();
	import Footer from '$lib/components/layoutComponents/Footer.svelte';
</script>

<svelte:head>
	<script src="https://kit.fontawesome.com/bb271890d7.js" crossorigin="anonymous"></script>
	<script
		async
		src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-5113481215151349"
		crossorigin="anonymous"
	></script>
</svelte:head>

<Header />
<div class="mt-10"></div>
{@render children()}

<Footer />
