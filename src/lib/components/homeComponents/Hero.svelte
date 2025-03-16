<script>
	import rocketLogo from '$lib/img/rocket.svg';
</script>

<section class="hero min-h-screen">
	<div
		class="hero-content container mx-auto flex flex-col items-center md:flex-row md:px-24 md:py-10"
	>
		<div
			class="md:w-1.5/2 mt-5 mb-16 flex flex-col items-center text-center md:mt-0 md:mb-0 md:items-start md:pr-16 md:text-left lg:flex-grow lg:pr-24"
		>
			<h1
				class="mb-6 text-3xl leading-9 font-extrabold tracking-tight sm:text-4xl sm:leading-10 md:text-5xl md:leading-normal"
			>
				Building digital <br />products &amp; brands.
			</h1>
			<p class="mb-10 pr-2 pl-2 leading-relaxed md:pl-0">
				We create amazing open-source projects that empower developers and foster collaboration.
			</p>
			<div class="flex justify-center font-semibold">
				<a
					href="#"
					class="inline-flex rounded border-0 bg-gradient-to-l from-[#1a2980] to-[#26d0ce] px-6 py-2 text-lg text-white hover:bg-gradient-to-r focus:outline-none"
					>Start Exploring
				</a>
				<a
					href="https://github.com/SmrtMrktX/"
					target="_blank"
					class="bg-base-content text-base-100 hover:bg-base-100 hover:text-base-content ml-4 inline-flex rounded border-0 px-6 py-2 text-lg duration-700

 hover:scale-125 focus:outline-none">GitHub</a
				>
			</div>
		</div>
		<div class="mb-5 w-3/6 md:mb-0 md:w-1/2 lg:w-full lg:max-w-lg">
			<img
				class="animate-[bounce_3s_ease-in-out_infinite] rounded object-cover object-center"
				alt="hero"
				src={rocketLogo}
			/>
		</div>
	</div>
</section>
