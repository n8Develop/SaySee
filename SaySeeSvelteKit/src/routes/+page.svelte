<script>
	import MainPageCarousel from './components/MainPage/mainPageCarousel.svelte';
	import MainPageImageGrid from './components/MainPage/mainPageImageGrid.svelte';
	import MainPageLatestImage from './components/MainPage/mainPageLatestImage.svelte';
</script>

<main>
	<div class="container">
		<MainPageCarousel />

		<MainPageLatestImage />
		<MainPageImageGrid />
	</div>
</main>

<style>
	main {
		font-family: sans-serif;
		text-align: center;
	}

	.container {
		display: grid;
		grid-template-rows: repeat(3, 33% [row-start]);
	}
</style>
