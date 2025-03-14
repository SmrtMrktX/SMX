<script>
	import sveltxLogo from '$lib/img/sveltxlogo.png';
	import testxLogo from '$lib/img/testxLogo.png';
	import nextxLogo from '$lib/img/nextxLogo.webp';
</script>

<div class="mx-auto mb-20 max-w-6xl p-6 text-center">
	<h2 class="my-12 text-center text-4xl font-extrabold sm:text-5xl">More Of Our Projects</h2>
	<div
		class="gr mx-auto max-w-3xl items-stretch space-y-4 text-left sm:flex sm:space-y-0 sm:space-x-8 sm:text-center"
	>
		<a
			class="border-opacity-10 hover:border-opacity-0 flex w-full items-center rounded-xl border px-4 py-6 duration-200 hover:no-underline hover:shadow-lg sm:flex-col sm:hover:shadow-2xl"
			href="https://sveltx.vercel.app"
			target="_blank"
		>
			<img class="mr-4 w-12 sm:mr-0 sm:h-32 sm:w-32" src={sveltxLogo} alt="Sveltx logo" />
			<div>
				<div class="font-semibold sm:mt-4 sm:mb-2">Sveltx</div>
				<div class="text-sm opacity-75">
					Sveltx a modern, feature-rich template for building scalable and performant applications
					using SvelteKit.
				</div>
			</div>
		</a>
		<a
			class="border-opacity-10 hover:border-opacity-0 dark:hover:bg-opacity-10 flex w-full items-center rounded-xl border px-4 py-6 duration-200 hover:no-underline hover:shadow-lg sm:flex-col sm:hover:shadow-2xl"
			href="https://testx-smx.vercel.app"
			target="_blank"
		>
			<img class="mr-4 w-12 rounded-4xl sm:mr-0 sm:h-32 sm:w-32" src={testxLogo} alt="Testx logo" />
			<div>
				<div class="font-semibold sm:mt-4 sm:mb-2">Testx</div>
				<div class="text-sm opacity-75">
					"Empowering Future Testers: A Comprehensive Software Testing Education Platform"
				</div>
			</div>
		</a>
		<a
			class="border-opacity-10 hover:border-opacity-0 dark:hover:bg-opacity-10 flex w-full items-center rounded-xl border px-4 py-6 duration-200 hover:no-underline hover:shadow-lg sm:flex-col sm:hover:shadow-2xl"
			href="#"
			target="_blank"
		>
			<img class="mr-4 w-12 rounded-4xl sm:mr-0 sm:h-32 sm:w-32" src={nextxLogo} alt="Next-X" />
			<div>
				<div class=" font-semibold sm:mt-4 sm:mb-2">Next X</div>
				<div class="text-sm opacity-75">
					Next-X: An open-source Tailwind CSS UI library with customizable, ready-to-use components
					for faster development.
				</div>
			</div>
		</a>
	</div>
</div>
