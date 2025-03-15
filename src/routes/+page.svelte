<script>
	import Hero from '$lib/components/homeComponents/Hero.svelte';
	import Poweredby from '$lib/components/homeComponents/Poweredby.svelte';
	import HowWeWork from '$lib/components/homeComponents/HowWeWork.svelte';
	import About from '$lib/components/homeComponents/About.svelte';
	import Services from '$lib/components/homeComponents/Services.svelte';
</script>

<svelte:head>
	<title>SMRT MRKT X</title>
	<meta
		name="description"
		content="SMX - SMRT MRKT X - OFFICIAL WEBSITE © - We create amazing open-source projects that empower developers and foster collaboration."
	/>
</svelte:head>

<Hero />

<Services />

<About />

<HowWeWork />

<Poweredby />
