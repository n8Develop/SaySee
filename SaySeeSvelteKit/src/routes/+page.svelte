<script>
	import MainPageCarousel from 'MainPage/mainPageCarousel.svelte';
	import MainPageImageGrid from 'MainPage/mainPageImageGrid.svelte';
	import MainPageLatestImage from 'MainPage/mainPageLatestImage.svelte';
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
