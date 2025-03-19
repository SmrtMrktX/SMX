<script>
	import sveltxlogo from '$lib/img/products/sveltxlogo.png';
</script>

<div
	class="bg-base-200 relative mx-auto flex max-w-screen-xl flex-col items-center p-8 sm:px-6 md:flex-row"
>
	<div class="flex items-center py-5 md:w-1/2 md:pt-10 md:pr-10 md:pb-20">
		<div class="text-left">
			<h2
				class="text-4xl leading-10 font-extrabold tracking-tight sm:text-5xl sm:leading-none md:text-6xl"
			>
				<span class="font-bold text-red-600">Sveltx</span>
				<span class=" rounded-full text-xl font-semibold">0.0.1</span>
			</h2>
			<p class="mx-auto mt-3 max-w-md text-base sm:text-lg md:mt-5 md:max-w-3xl md:text-xl">
				🚀 Sveltx – a modern, feature-rich template for building scalable and high-performance web
				applications with the SvelteKit framework and the DaisyUI library.
			</p>
			<div class="mt-5 sm:flex md:mt-8">
				<div class="rounded-md shadow">
					<a
						href="https://sveltx.vercel.app/"
						target="_blank"
						class="focus:shadow-outline-blue flex w-full items-center justify-center rounded-md border border-transparent bg-red-600 px-8 py-3 text-base leading-6 font-medium text-white transition duration-150 ease-in-out hover:bg-green-700 focus:outline-none md:px-10 md:py-4 md:text-lg"
					>
						Live
					</a>
				</div>
				<div class="mt-3 rounded-md shadow sm:mt-0 sm:ml-3">
					<a
						href="https://github.com/SmrtMrktX/Sveltx"
						target="_blank"
						class="focus:shadow-outline-blue flex w-full items-center justify-center rounded-md border border-transparent bg-white px-8 py-3 text-base leading-6 font-medium text-red-600 transition duration-150 ease-in-out hover:text-green-700 focus:outline-none md:px-10 md:py-4 md:text-lg"
					>
						Contribute
					</a>
				</div>
			</div>
		</div>
	</div>
	<div class="flex items-center py-5 md:w-1/2 md:pt-10 md:pb-20 md:pl-10">
		<div class="relative w-full rounded p-3 md:p-8">
			<div class="hero-content w-full">
				<img src={sveltxlogo} alt="Sveltx logo" />
			</div>
		</div>
	</div>
</div>
