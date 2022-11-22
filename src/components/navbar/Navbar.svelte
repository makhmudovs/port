<script>
	let isOpen = false;
</script>

<nav class="navbar relative bg-white shadow dark:bg-gray-800">
	<div class="container px-6 py-3 mx-auto md:flex md:items-center md:justify-between">
		<div class="flex items-center justify-between">
			<div>
				<a
					class="text-2xl font-bold text-gray-800 transition-colors duration-300 transform dark:text-white lg:text-3xl hover:text-gray-700 dark:hover:text-gray-300"
					href="#">Alex</a
				>
			</div>

			<!-- Mobile menu button -->
			<div class="flex md:hidden">
				<button
					on:click={() => (isOpen = !isOpen)}
					type="button"
					class="text-gray-500 dark:text-gray-200 hover:text-gray-600 dark:hover:text-gray-400 focus:outline-none focus:text-gray-600 dark:focus:text-gray-400"
					aria-label="toggle menu"
				>
					<svg
						xmlns="http://www.w3.org/2000/svg"
						class={`${isOpen ? 'hidden' : ''} w-6 h-6`}
						fill="none"
						viewBox="0 0 24 24"
						stroke="currentColor"
						stroke-width="2"
					>
						<path stroke-linecap="round" stroke-linejoin="round" d="M4 8h16M4 16h16" />
					</svg>

					<svg
						class={`${isOpen ? '' : 'hidden'} w-6 h-6`}
						xmlns="http://www.w3.org/2000/svg"
						fill="none"
						viewBox="0 0 24 24"
						stroke="currentColor"
						stroke-width="2"
					>
						<path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
					</svg>
				</button>
			</div>
		</div>
		<!-- Mobile Menu open: "block", Menu closed: "hidden" -->
		<div
			class={`${
				isOpen ? 'translate-x-0 opacity-100 ' : 'opacity-0 -translate-x-full'
			} absolute inset-x-0 z-20 w-full md:w-auto px-6 py-4 transition-all duration-300 ease-in-out bg-white dark:bg-gray-800 md:mt-0 md:p-0 md:top-0 md:relative md:opacity-100 md:translate-x-0 md:flex md:items-center md:justify-between`}
		>
			<div class="flex flex-col px-2 -mx-4 md:flex-row md:mx-10 md:py-0">
				<a
					href="#about"
					class="px-2.5 py-2 text-gray-700 transition-colors duration-300 transform rounded-lg dark:text-gray-200 hover:bg-gray-100 dark:hover:bg-gray-700 md:mx-2"
					>About</a
				>
				<a
					href="#portfolio"
					class="px-2.5 py-2 text-gray-700 transition-colors duration-300 transform rounded-lg dark:text-gray-200 hover:bg-gray-100 dark:hover:bg-gray-700 md:mx-2"
					>Portfolio</a
				>
				<a
					href="#contact"
					class="px-2.5 py-2 text-gray-700 transition-colors duration-300 transform rounded-lg dark:text-gray-200 hover:bg-gray-100 dark:hover:bg-gray-700 md:mx-2"
					>Cooperate</a
				>
				<div class="pl-2 block md:hidden">
					<button
						type="button"
						class="px-2.5 py-2 bg-orange-400 text-white transition-colors duration-300 transform rounded-lg dark:text-gray-200 hover:bg-gray-100 dark:hover:bg-gray-700 md:mx-2 text-left"
						>Contact Me</button
					>
				</div>
			</div>
		</div>
		<button
			type="button"
			class="text-white hidden md:block bg-orange-500 hover:bg-orange-600 focus:ring-4 focus:ring-orange-300 font-medium rounded-lg text-sm px-5 py-2.5 mr-2 mb-2 focus:outline-none "
			>Contact Me</button
		>
	</div>
</nav>

<style>
	.navbar {
		font-family: 'Open Sans', sans-serif;
	}
</style>
