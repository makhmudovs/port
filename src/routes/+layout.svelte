<script>
	// @ts-nocheck

	import Navbar from '../components/navbar/Navbar.svelte';
	import '../app.postcss';
</script>

<svelte:head>
	<link rel="preconnect" href="https://fonts.googleapis.com" />
	<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
	<link
		href="https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,500;0,600;0,700;0,800;1,400;1,500;1,600;1,700;1,800&family=Raleway:ital,wght@0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap"
		rel="stylesheet"
	/>
	<script src="https://cdn.jsdelivr.net/npm/vanilla-lazyload@17.8.3/dist/lazyload.min.js"></script>
</svelte:head>
<div class="layout">
	<Navbar />
	<div class="dark:bg-gray-800">
		<slot />
	</div>
</div>

<style>
	.layout {
		font-family: 'Raleway', sans-serif;
	}
</style>
