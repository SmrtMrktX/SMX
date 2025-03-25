<script>
	import desktopApp from '$lib/img/download/desktopapp.png';
</script>

<section class="hero min-h-screen">
	<div class="container mx-auto max-w-xl space-y-12 p-6 lg:max-w-7xl lg:px-8">
		<div>
			<h2 class="text-center text-3xl font-bold sm:text-5xl">SMX - Desktop</h2>
			<p class="mx-auto mt-4 max-w-3xl text-center text-xl">
				Explore the latest features that enhance your learning experience and make it even more
				exciting.
			</p>
		</div>
		<div class="grid lg:grid-cols-2 lg:items-center lg:gap-8">
			<div>
				<div class="mt-4 space-y-12">
					<div class="flex">
						<div class="flex-shrink-0">
							<div class="flex h-12 w-12 items-center justify-center rounded-md">
								<svg
									xmlns="http://www.w3.org/2000/svg"
									width="24"
									height="24"
									viewBox="0 0 24 24"
									fill="none"
									stroke="green"
									stroke-width="2"
									stroke-linecap="round"
									stroke-linejoin="round"
									class="lucide lucide-rocket"
								>
									<path
										d="M4.5 16.5c-1.5 1.26-2 5-2 5s3.74-.5 5-2c.71-.84.7-2.13-.09-2.91a2.18 2.18 0 0 0-2.91-.09z"
									>
									</path>
									<path
										d="m12 15-3-3a22 22 0 0 1 2-3.95A12.88 12.88 0 0 1 22 2c0 2.72-.78 7.5-6 11a22.35 22.35 0 0 1-4 2z"
									>
									</path>
									<path d="M9 12H4s.55-3.03 2-4c1.62-1.08 5 0 5 0"></path>
									<path d="M12 15v5s3.03-.55 4-2c1.08-1.62 0-5 0-5"></path>
								</svg>
							</div>
						</div>
						<div class="ml-4">
							<h4 class="leadi text-lg font-medium">
								Cross-platform Software | Windows - Linux - macOS
							</h4>
							<p class="mt-2">
								Discover the multi-platform software, is designed to work on several computing
								platforms such as different operating systems or devices.
							</p>
						</div>
					</div>
					<div class="flex">
						<div class="flex-shrink-0">
							<div class="flex h-12 w-12 items-center justify-center rounded-md">
								<svg
									xmlns="http://www.w3.org/2000/svg"
									width="24"
									height="24"
									viewBox="0 0 24 24"
									fill="none"
									stroke="blue"
									stroke-width="2"
									stroke-linecap="round"
									stroke-linejoin="round"
									class="lucide lucide-bookmark-plus"
								>
									<path d="m19 21-7-4-7 4V5a2 2 0 0 1 2-2h10a2 2 0 0 1 2 2v16z"></path>
									<line x1="12" x2="12" y1="7" y2="13"></line>
									<line x1="15" x2="9" y1="10" y2="10"></line>
								</svg>
							</div>
						</div>
						<div class="ml-4">
							<h4 class="leadi text-lg font-medium">Interactive Learning Resources</h4>
							<p class="mt-2">
								Access an extensive library of interactive resources that make your learning journey
								engaging and interactive.
							</p>
						</div>
					</div>

					<div class="flex">
						<div class="flex-shrink-0">
							<div class="flex h-12 w-12 items-center justify-center rounded-md">
								<svg
									xmlns="http://www.w3.org/2000/svg"
									width="24"
									height="24"
									viewBox="0 0 24 24"
									fill="none"
									stroke="purple"
									stroke-width="2"
									stroke-linecap="round"
									stroke-linejoin="round"
									class="lucide lucide-file-question"
								>
									<path d="M14.5 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V7.5L14.5 2z"
									></path>
									<path d="M10 10.3c.2-.4.5-.8.9-1a2.1 2.1 0 0 1 2.6.4c.3.4.5.8.5 1.3 0 1.3-2 2-2 2"
									></path>
									<path d="M12 17h.01"></path>
								</svg>
							</div>
						</div>
						<div class="ml-4">
							<h4 class="leadi text-lg font-medium">MIT License</h4>
							<p class="mt-2">
								The MIT License is a permissive free software license that allows users to use,
								copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
								software,
							</p>
						</div>
					</div>
				</div>
			</div>
			<div aria-hidden="true" class="mt-10 lg:mt-0">
				<img
					width="600"
					height="600"
					src={desktopApp}
					class="dark-bg-gray-500 mx-auto rounded-lg shadow-lg"
					style="color:transparent"
					alt="desktop app"
				/>
			</div>
		</div>
		<div class="mt-20 flex justify-center">
			<a href="https://github.com/SmrtMrktX/SMX-desktop" target="_blank"
				><button class="p-2">Discover</button></a
			>
		</div>
	</div>
</section>

<style>
	button {
		border-radius: 8px;
		border: 1px solid transparent;
		font-size: 1em;
		font-weight: 500;
		font-family: inherit;
		color: #0f0f0f;
		background-color: whitesmoke;

		box-shadow: 0 2px 2px rgba(0, 0, 0, 0.2);
		cursor: pointer;
	}
	button:hover {
		border-color: #396cd8;
	}
</style>
