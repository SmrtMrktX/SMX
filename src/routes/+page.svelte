<script>
	import rocketLogo from '$lib/img/rocket.svg';
</script>

<svelte:head>
	<title>SMRT MRKT X</title>
	<meta
		name="description"
		content="SMX - SMRT MRKT X - OFFICIAL WEBSITE © - We create amazing open-source projects that empower developers and foster collaboration."
	/>
</svelte:head>

<section class="hero min-h-screen">
	<div
		class="hero-content container mx-auto flex flex-col items-center md:flex-row md:px-24 md:py-10"
	>
		<div
			class="md:w-1.5/2 mt-5 mb-16 flex flex-col items-center text-center md:mt-0 md:mb-0 md:items-start md:pr-16 md:text-left lg:flex-grow lg:pr-24"
		>
			<h1
				class="mb-3 text-2xl leading-9 font-extrabold tracking-tight sm:text-4xl sm:leading-10 md:text-5xl md:leading-normal"
			>
				Building digital <br />products &amp; brands.
			</h1>
			<p class="mb-8 pr-2 pl-2 leading-relaxed md:pl-0">
				We create amazing open-source projects that empower developers and foster collaboration.
			</p>
			<div class="flex justify-center font-semibold">
				<a
					href="#"
					class="inline-flex rounded border-0 bg-emerald-600 from-[#4F46E5] to-[#E114E5] px-6 py-2 text-lg text-white hover:bg-gradient-to-r hover:bg-clip-text hover:text-transparent focus:outline-none"
					>Start Exploring
				</a>
				<a
					href="https://github.com/SmrtMrktX/"
					target="_blank"
					class="ml-4 inline-flex rounded border-0 bg-gray-100 px-6 py-2 text-lg text-gray-700 hover:bg-gray-200 focus:outline-none"
					>Github</a
				>
			</div>
		</div>
		<div class="mb-5 w-3/6 md:mb-0 md:w-1/2 lg:w-full lg:max-w-lg">
			<img class="rounded object-cover object-center" alt="hero" src={rocketLogo} />
		</div>
	</div>
</section>
